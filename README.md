# TASK-2-CPP-MULTITHREADED-FILE-COMPRESSION-TOOL
COMPANY: CODTECH IT SOLUTIONS
NAME: PRAKRITI ROY
INTERN ID: CT04DN488
DOMAIN: C++ PROGRAMMING
DURATION: 4 WEEKS
MENTOR: NEEL SANTOSH

DESCRIPTION:
This C++ program performs Run-Length Encoding (RLE) compression and decompression on a text file using multithreading. RLE is a simple lossless data compression technique that replaces sequences of repeated characters with a single character followed by its count (e.g., "aaaabb" becomes "4a2b").

Key Components:

1. RLE Compression (rleCompress):

Iterates through the input string.

Counts consecutive repeating characters.

Constructs a compressed string in the format count + character.

2. RLE Decompression (rleDecompress):

Reads the compressed string.

Extracts numeric counts followed by a character.

Reconstructs the original string using the count and character.

3. Threading with Mutex:

Two separate threads are launched: one for compression, one for decompression.

A mutex is used to avoid overlapping output in the console when threads print messages.

4. File Handling:

The user provides an input filename.

The program reads the content of that file, compresses it, and saves it to compressed_output.txt.

The compressed file is then decompressed and saved to decompressed_output.txt.

5. Multithreading:

std::thread is used to run compression and decompression in parallel.

The main() function waits for both threads to complete using join().

Summary:

This program demonstrates file I/O, basic string manipulation, RLE compression/decompression logic, and concurrent execution using threads and mutexes.

OUTPUT:
![Image](https://github.com/user-attachments/assets/d69c1c8c-7593-4849-9d05-3b0f4fd8b7f9)
