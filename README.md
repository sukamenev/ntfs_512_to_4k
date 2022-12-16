# A program for correcting the boot and backup sectors of NTFS after cloning from a disk with a 512 sector to 4K.

## Install

`chmod a+x ntfs_512_to_4k`

## Examples

Examples of using:

Show information from the NTFS boot sector and its copy.

  `./ntfs_512_to_4k show /dev/nvme0n1p5`

Convert information in NTFS boot sectors from 512 to 4K sectors (after cloning)

`./ntfs_512_to_4k fix /dev/nvme0n1p5`

Revert changes in boot sectors from 4K to 512B sectors

`./ntfs_512_to_4k unfix /dev/nvme0n1p5`
