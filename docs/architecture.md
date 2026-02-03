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

## Data Flow Overview

1. Input image is provided to the system through software.
2. Software performs resizing and normalization.
3. Preprocessed data is transferred to the FPGA accelerator.
4. FPGA accelerator performs CNN inference.
5. Results are sent back to software for classification output.

## Open Questions

- How is data transferred between software and FPGA?
- What image size and data format are used?
- Which CNN layers are accelerated in hardware?

