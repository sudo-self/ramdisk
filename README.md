<h1 align="center">SSH Ramdisk Script</h1>

<p align="center">
  <a href="https://github.com/verygenericname/SSHRD_Script/graphs/contributors" target="_blank">
    <img src="https://img.shields.io/github/contributors/verygenericname/SSHRD_Script.svg" alt="Contributors">
  </a>
  <a href="https://github.com/verygenericname/SSHRD_Script/commits/main" target="_blank">
    <img src="https://img.shields.io/github/commit-activity/w/verygenericname/SSHRD_Script.svg" alt="Commits">
  </a>
</p>

<p align="center">
Create and boot a SSH ramdisk on checkm8 devices.
</p>

---
## Warning
This was used in palera1n.sh, this is no longer gonna be maintained.
# Prerequsites

1. A computer running macOS/linux
2. A checkm8 device (A7-A11)

# Usage

1. Clone and cd into this repository: `git clone https://github.com/verygenericname/SSHRD_Script --recursive && cd SSHRD_Script`
    - If you have cloned this before, run `cd SSHRD_Script && git pull` to pull new changes
2. Run `./sshrd.sh <iOS version for ramdisk>`, **without** the `<>`.
3. Place your device into DFU mode
    - A11 users, go to recovery first, then DFU.
4. Run `./sshrd.sh boot` to boot the ramdisk
5. Run `./sshrd.sh ssh` to connect to SSH on your device
6. Finally, to mount the filesystems, run `mount_filesystems`  
    - /var is mounted to /mnt2 in the ssh session.
    - /private/preboot is mounted to /mnt6.

# Other commands

- Reset your device: `./sshrd.sh reset`
- Dump onboard blobs: `./sshrd.sh dump-blobs`
- Delete old SSH ramdisk: `./sshrd.sh clean`

![ssh](https://user-images.githubusercontent.com/119916323/230703244-d8c04517-9de9-408d-8c8d-3571932ea1ab.jpg)![IMG_1082](https://user-images.githubusercontent.com/119916323/230703275-bdaf060f-1f3d-44a2-98cd-aa6a5f7d4e5d.jpg)


