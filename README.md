I have implemented a very simple file system checker using defined supernode, inode and data bitmap structure. This project implements a consistency checker for a Very Simple File System (VSFS). The checker verifies and repairs inconsistencies in a disk image, ensuring the integrity of core file system components. It validates the superblock, inode and data block bitmaps, and inode structures. Additionally, it detects and fixes errors such as:

Incorrect magic number in the superblock

Bitmap mismatches for allocated/free inodes and blocks

Invalid direct or indirect block references in inodes

Unused inodes with non-zero fields

Duplicate block references

The tool is written in C and provides both detection and repair capabilities, helping to simulate real-world file system checkers
