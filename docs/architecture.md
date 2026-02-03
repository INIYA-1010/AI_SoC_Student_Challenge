# Architecture Overview

This project aims to implement a hardware-accelerated CNN on FPGA.

The system consists of:
- Input image preprocessing in software
- CNN acceleration using FPGA logic
- Output classification in software

Data flows from preprocessing to hardware accelerator and back to software.

## Initial Block Description

- Preprocessing: Converts input image into CNN-compatible format.
- FPGA Accelerator: Executes CNN layers for faster inference.
- Postprocessing: Interprets accelerator output.
