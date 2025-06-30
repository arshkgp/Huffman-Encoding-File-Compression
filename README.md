# Huffman Encoding File Compression

## Overview

This project implements Huffman encoding in C++ for efficient, lossless file and directory compression. It reduces storage space while preserving complete data integrity, supporting a variety of file types and cross-platform compatibility.

## Features

- **Lossless Compression:** Achieves file size reduction using the Huffman algorithm without losing any information.
- **Directory Compression:** Recursively compresses all files in a directory, maintaining the original folder structure.
- **File Type Support:** Handles different file types, including text and images, adapting the encoding as needed.
- **Cross-Platform:** Compatible with Windows, Linux, and macOS using standard C++ libraries.

## How It Works

1. **Frequency Analysis:** Scans each file to count character frequencies.
2. **Huffman Tree Construction:** Builds a binary tree using a priority queue, assigning shorter codes to more frequent characters.
3. **Encoding:** Replaces each character in the file with its Huffman code, producing a compressed output file.
4. **Directory Traversal:** Recursively processes all files in a directory, compressing each one individually and preserving the directory structure.

## Technical Details

- **Data Structures:** Utilizes priority queues and binary trees for efficient Huffman tree construction and code assignment.
- **File Handling:** Uses the C++ `<filesystem>` library for directory and file management.
- **Efficiency:** Processes files in binary mode for speed and memory efficiency.

## Usage

### Compress a Single File

string inputPath = "input.txt";
string outputPath = "output.huff";
compressFile(inputPath, outputPath);


### Compress a Directory

string inputDirPath = "input_directory";
string outputDirPath = "output_directory";
compressDirectory(inputDirPath, outputDirPath);


## Requirements

- C++17 or later
- Standard Template Library (STL)
- Compatible with GCC, Clang, or MSVC compilers

## Applications

- **Archiving:** Reduce storage space for backups and archives.
- **File Transfer:** Send smaller files over networks.
- **Storage Optimization:** Make better use of disk space for various file types.

---

This project demonstrates practical use of advanced C++ concepts, including efficient data structures, file I/O, and directory management, to deliver a robust solution for lossless file compression using Huffman encoding.
