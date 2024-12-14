# format-thumb
Linux Commands to Format a Thumb Drive

```
lsblk

sudo umount /dev/sdf1

sudo parted /dev/sdf mklabel msdos

sudo parted /dev/sdf "mkpart primary fat32 0% -1s"

sudo mkdosfs -F 32 /dev/sdf1
```
