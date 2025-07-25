# btrfs inspect-internal

> Query internal information of a btrfs filesystem.
> More information: <https://btrfs.readthedocs.io/en/latest/btrfs-inspect-internal.html>.

- Print superblock's information:

`sudo btrfs {{[i|inspect-internal]}} {{[dump-s|dump-super]}} {{path/to/partition}}`

- Print superblock's and all of its copies' information:

`sudo btrfs {{[i|inspect-internal]}} {{[dump-s|dump-super]}} {{[-a|--all]}} {{path/to/partition}}`

- Print filesystem's metadata information:

`sudo btrfs {{[i|inspect-internal]}} {{[dump-t|dump-tree]}} {{path/to/partition}}`

- Print list of files in inode `n`-th:

`sudo btrfs {{[i|inspect-internal]}} {{[i|inode-resolve]}} {{n}} {{path/to/btrfs_mount}}`

- Print list of files at a given logical address:

`sudo btrfs {{[i|inspect-internal]}} {{[lo|logical-resolve]}} {{logical_address}} {{path/to/btrfs_mount}}`

- Print stats of root, extent, csum and fs trees:

`sudo btrfs {{[i|inspect-internal]}} {{[t|tree-stats]}} {{path/to/partition}}`
