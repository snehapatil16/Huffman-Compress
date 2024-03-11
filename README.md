# Huffman Compression/Decompression

This repository contains a C program for compressing or decompressing a text file using Huffman compression.

## Overview

The program is divided into two files:

- `hcompress.c`: This file contains the main function and methods for encoding and decoding files using Huffman coding.
- `linkedList.c` and `linkedList.h`: These files contain the implementation and header for a linked list data structure used in the Huffman tree construction.

## Usage

### Compiling

Compile the program using "gcc" with all warnings turned on (-Wall flag) on a Linux operating system.

### Running

To compress a file:
```
hcompress -e filename
```
This creates a compressed file called "filename.huf".

To decompress a compressed file:
```
hcompress -d filename.huf
```
This creates a decompressed file called "filename.huf.dec".

## Huffman Compression/Decompression

The core functionality of the program revolves around Huffman coding, a technique for lossless data compression.

### Encoding

- `createFreqTable`: Reads a generic text file and counts the frequency of each character.
- `createHuffmanTree`: Constructs the Huffman tree from the frequency table using a linked list.
- `encodeFile`: Encodes a given file using Huffman coding based on the constructed tree.

### Decoding

- `decodeFile`: Decodes a compressed file using Huffman coding based on the constructed tree.

These methods allow for efficient compression and decompression of text files while maintaining lossless data integrity.
