# Composer-or-Conductor-

## Overview

This project investigates how conductors and orchestras influence a piece's emotional expression compared to the composer's original intent. Using machine learning and audio analysis, it processes recordings to quantify emotional attributes across different performances of the same classical pieces.

## Pipeline Structure

The pipeline consists of three main phases:

1. **Data Collection** (`Data Collection.ipynb`)
  - Scrapes metadata from IMSLP
  - Collects performance links 
  - Creates structured dataset mapping pieces to recordings

2. **Audio Processing** (`Audio Conversion Process.ipynb`)
  - Downloads recordings using yt-dlp
  - Converts media to standardized audio format
  - Handles batch processing of large audio files

3. **Analysis & Prediction** (`Model Predictions.ipynb`) 
  - Segments audio into analyzable chunks
  - Extracts audio features using librosa (MFCCs, chroma, tempo)
  - Generates emotional predictions using Claude API
  - Compares conductor vs composer influence

## Tools Used
- yt-dlp for audio downloads
- librosa for audio feature extraction  
- Claude API for emotional analysis
- Python data processing libraries
