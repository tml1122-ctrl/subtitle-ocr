# Subtitle OCR

A video subtitle extraction pipeline based on PaddleOCR.

## Overview

This project extracts hardcoded subtitles from video frames using
pre-generated subtitle regions and timing information.

## Pipeline

Video
→ Subtitle Region
→ ROI Cropping
→ PaddleOCR
→ Subtitle Text
→ SRT

## Features

- GPU-accelerated PaddleOCR
- Subtitle region based ROI extraction
- Multi-line subtitle recognition
- SRT text replacement
- JSON-based intermediate data

## Requirements

- Python
- OpenCV
- PaddlePaddle GPU
- PaddleOCR
- PySRT

## Output

The recognized subtitle text is written back to an SRT subtitle file.

## Limitations

The current prototype assumes that subtitle timing and region information
are available as input.