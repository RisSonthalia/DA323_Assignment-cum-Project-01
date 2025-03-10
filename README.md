# DA323: Multimodal Data Analysis and Learning 2.0  
**Assignment-cum-Project-01 (Jan-May 2025, IIT Guwahati)**

## Overview

This repository contains the complete project submission for DA323: Multimodal Data Analysis and Learning 2.0. The project focuses on scalable data collection, multimodal analysis, and computational matching techniques across various modalities (image, text, audio, and weather data). It also includes a multimodal challenge on analyzing national flags and anthems to uncover cultural correlations.

## Repository Structure

```
DA323-Multimodal-Data-Analysis/
├── TASK1/                # Scalable Data Collection
│   ├── Task_A/           # Image Dataset Collection
│   │   ├── datasets/     # Downloaded images and metadata CSV files
│   │   ├── datasheets/   # Datasheet for the Image Dataset
│   │   └── notebooks/    # Jupyter Notebooks for Task A
│   ├── Task_B/           # Text Dataset Collection
│   │   ├── datasets/     # Collected text files (20 categories)
│   │   ├── datasheets/   # Datasheet for the Text Dataset
│   │   └── notebooks/    # Jupyter Notebooks for Task B
│   ├── Task_C/           # Audio Dataset Collection
│   │   ├── datasets/     # Recorded audio files (WAV/MP3) with metadata
│   │   ├── datasheets/   # Datasheet for the Audio Dataset
│   │   └── notebooks/    # Jupyter Notebooks for Task C
│   ├── Task_D/           # Weather Dataset Collection
│   │   ├── datasets/     # Weather data CSV files for 20 Indian cities
│   │   ├── datasheets/   # Datasheet for the Weather Dataset
│   │   └── notebooks/    # Jupyter Notebooks for Task D
│   └── Task_E/           # Analyzing India with Data
│       ├── datasets/     # Selected dataset from data.gov.in
│       ├── datasheets/   # Datasheet for the dataset
│       └── notebooks/    # Jupyter Notebooks for Task E
├── TASK3/                # Analyzing Flags and Anthems
│   ├── datasets/         # Multimodal datasets:
│   │   ├── flags_png/    # National flag images
│   │   ├── anthem_translations.json  # Anthem text translations
│   │   └── anthem_mp3/   # Anthem audio files
│   ├── datasheets/       # Datasheet for the Multimodal Flags & Anthems Dataset
│   └── notebooks/        # Jupyter Notebooks for Parts A to E (visual, textual, audio, and multimodal analyses)
└── README.md             # This file
```

## Contents

### TASK1: Scalable Data Collection
Contains scripts, Jupyter Notebooks, datasets, and datasheets for scalable data collection:

- **Task_A: Image Dataset Collection**
  - Collected images for 20 different categories using automated scripts
  - Each category contains 50 images with metadata (URL, filename, resolution)
  - Dataset is organized into labeled folders
  - Use Case: Object recognition, image classification, and visual search applications

- **Task_B: Text Dataset Collection**
  - Web crawlers extracted articles from three websites for each of 20 categories
  - Cleaned text using NLP techniques and stored in organized text files
  - Use Case: Sentiment analysis, topic modeling, and natural language processing research

- **Task_C: Audio Dataset Collection**
  - Recorded 30 audio streams from online AM/FM radio stations (30-90 seconds each)
  - Metadata includes station name, timestamp, and duration
  - Use Case: Audio signal processing, music classification, and speech recognition research

- **Task_D: Weather Dataset Collection**
  - Collected historical and real-time weather data for 20 Indian cities using OpenWeatherMap API
  - Data includes temperature, humidity, wind speed, etc., stored in CSV format
  - Use Case: Weather trend analysis, climatology studies, and urban planning

- **Task_E: Analyzing India with Data**
  - Analysis of selected datasets from data.gov.in
  - Exploratory data analysis and visualization

### TASK3: Analyzing Flags and Anthems
Contains datasets and analysis related to national flags and anthems:

- **Visual Analysis:**
  - Extracted flag features using traditional techniques and CNN-based methods
  - Analyzed aspect ratios, color histograms, and edge detection patterns

- **Textual Analysis:**
  - Processed national anthem translations with NLP techniques
  - Explored linguistic features and thematic patterns

- **Audio Analysis:**
  - Analyzed anthem audio files using waveform visualization, spectrograms, and MFCCs
  - Extracted tempo and other musical features

- **Multimodal Correlation:**
  - Integrated visual, textual, and audio features to investigate cross-modal correlations
  - Built generative models to explore relationships between flag features and anthem characteristics

## How to Use

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/DA323-Multimodal-Data-Analysis.git
   cd DA323-Multimodal-Data-Analysis
   ```

2. **Install Dependencies:**
   Install required libraries via:
   ```bash
   pip install -r requirements.txt
   ```
   (Dependencies include numpy, pandas, matplotlib, seaborn, torch, torchvision, opencv-python, beautifulsoup4, selenium, etc.)

3. **Explore the Notebooks:**
   Open Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
   Navigate to the desired task folder (e.g., TASK1/Task_A for image data collection or TASK3/notebooks for flag and anthem analysis) and run the notebooks.

4. **Review Datasheets:**
   Each task folder contains a datasheet.md that documents the dataset details, collection methods, and use cases.

## Use Cases

### Multimodal Research:
Supports studies in cross-modal correlation, generative modeling, and feature extraction across images, text, audio, and weather data.

### Educational Resource:
Provides comprehensive examples of automated data collection, preprocessing, and analysis for diverse data modalities.

### Cultural & Historical Analysis:
Enables investigation into national identity and cultural symbolism through the analysis of flags and anthems.

## 9. Contact Information

For any questions, issues, or further collaboration ,please contact:

- **Project Lead:** Rishab Sonthalia
- **Institution:** IIT Guwahati, DA323: Multimodal Data Analysis and Learning 2.0
- **Email:** s.rishab@iitg.ac.in
---

For further details, please refer to the individual datasheets and Jupyter Notebooks within each task folder.
