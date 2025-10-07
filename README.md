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
Image-Processing-MIPS
├── ImageProcessing.s # MIPS assembly source code
├── lenna.pgm # Test input image (512x512 grayscale)
├── textfile.pgm # Text-based PGM file used for blur/encryption tests
└── README.md # Project documentation


---

## How to Run
1. Open `ImageProcessing.s` in MARS.  
2. Make sure `lenna.pgm` and `textfile.pgm` are in the same directory.  
3. Assemble (`F3`) and run (`F5`).

### Output Files Generated
- `lenna_thresh.pgm` – result of thresholding  
- `lenna_rotation.pgm` – rotated image  
- `lenna_scale.pgm` – scaled image  
- `lenna_shear.pgm` – sheared image  
- `text_crypt.pgm` – blurred or encrypted text file  

### Viewing Results
Open the output `.pgm` files in an image viewer such as GIMP, IrfanView, or Visual Studio Code with an image preview extension.

---

## Concepts Demonstrated
- Image buffer manipulation in memory  
- Affine matrix transformations in assembly  
- Loop and branch optimization  
- File handling syscalls (13–16: open, read, write, close)  
- Threshold-based pixel classification  

---

## Example Workflow
1. Input: `textfile.pgm` (renders readable English text)  
2. Operation: Apply `cryptography` function (custom blur)  
3. Output: `text_crypt.pgm` (blurred or distorted text)  

The visual output should show blurred or altered text depending on the implemented algorithm.

---

## Author
Calvin Poruthur Raju  
Email: [calvinpraju@gmail.com]  
LinkedIn / GitHub: [https://www.linkedin.com/in/calvin-raju/]

---

## Keywords
MIPS Assembly, Image Processing, PGM, Affine Transform, Thresholding, Cryptography, Low-Level Programming

