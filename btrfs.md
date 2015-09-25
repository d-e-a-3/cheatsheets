# Btrfs

Command | Description
------- | -----------
**`btrfs subvolume create /btrfs/sub1`** | Create subvolume /sub1 under top-level 'btrfs' subvolume
**`btrfs subvolume list /btrfs`** | List subvolumes
**`btrfs subvolume get-default /btrfs`** | Get default subvolume ID
**`mount -o subvolid=261 /dev/sdd1 /btrfs/`** | Mount subvolume by itselfs, without the top-level subvolume.
**`btrfs subvolume snapshot /btrfs/sub1 /btrfs/sub1/snapshot`** | Create snapshot of subvolume.
**`btrfs filesystem show`** | Show information of all the btrfs filesystem both mounted and unmounted.
