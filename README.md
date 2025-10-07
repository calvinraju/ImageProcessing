# Image Processing in MIPS Assembly

## Overview
This project demonstrates low-level image processing using MIPS assembly.  
It performs thresholding, matrix transformations, and basic cryptographic blurring on grayscale images stored in the `.pgm` (Portable GrayMap) format.

By working directly with pixel data, it shows how image transformations can be achieved through manual memory management, matrix arithmetic, and file I/O syscalls in MIPS.

---

## Features
- Thresholding — Converts grayscale images to binary (black and white) using a set intensity threshold.  
- Matrix Transformations — Performs scaling, rotation, and shearing via affine transformation matrices.  
- Cryptography / Blur Simulation — Manipulates pixel data for encryption-like visual distortion.  
- File I/O in MIPS — Reads and writes `.pgm` image files using syscalls 13–16.  
- Automated Testing — Built-in test data for each function (threshold, transform, cryptography).

---

## Technologies
- Language: MIPS Assembly  
- Simulator: MARS MIPS Simulator  
- Image Format: PGM (P5, binary)  
- Files Used:
  - `lenna.pgm` — sample input image  
  - `textfile.pgm` — text-based input image for blur/encryption tests  

---

## Project Structure
