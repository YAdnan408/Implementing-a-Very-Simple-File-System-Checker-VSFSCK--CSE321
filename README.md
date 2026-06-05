# VSFSCK: Very Simple File System Checker

## Description
This project implements a consistency checker for a Very Simple File System (VSFS). The checker verifies and repairs inconsistencies in a disk image, ensuring the integrity of core file system components. It validates the superblock, inode and data block bitmaps, and inode structures.

### Detects and fixes errors such as:
1. Incorrect magic number in the superblock
2. Bitmap mismatches for allocated/free inodes and blocks
3. Invalid direct or indirect block references in inodes
4. Unused inodes with non-zero fields
5. Duplicate block references

## How to Run

### 1. Compile
```bash
gcc -o vsfsck vsfsck.c
```

### 2. Run
```bash
./vsfsck <fs_image>
```
