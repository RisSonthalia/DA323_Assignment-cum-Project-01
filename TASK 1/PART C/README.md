# Datasheet for RadioStream_Chronicles Audio Dataset

This datasheet provides detailed documentation for the **RadioStream Chronicles Audio Dataset**, a collection of audio recordings captured from various publicly available online radio stations. The dataset was created as part of the DA323: Multimodal Data Analysis and Learning 2.0 project at IIT Guwahati (Jan-May 2025).

---

## 1. Overview
- **Dataset Name:** RadioStream_Chronicles  
- **Project:** DA323: Multimodal Data Analysis and Learning 2.0  
- **Version:** 1.0  
- **Date Created:** March 2025  
- **Creators:** Rishab Sonthalia ,IIT Guwahati 
- **Contact:** s.rishab@iitg.ac.in  

### 1.1 Purpose of Dataset
- **Research Goals:**  
  The dataset was developed to support scalable data collection techniques and facilitate multimodal analysis, including tasks such as audio-video matching and audio signal processing.
- **Use Case:**  
  It serves as a sample dataset for exploring automated audio collection, feature extraction, classification, and potential integration with other data modalities (e.g., text, images, structured weather data).

### 1.2 Intended Audience
- Researchers and practitioners in data science, machine learning, and multimodal analysis.
- Students and educators involved in data collection and preprocessing tasks.
- Developers working on audio signal processing or real-time data scraping applications.

---

## 2. Dataset Composition

### 2.1 Contents
- **Audio Files:**  
  - 30 audio recordings in MP3 format.
  - Each recording is sampled for a duration randomly chosen between 30 and 90 seconds.
- **Metadata:**  
  - A CSV file (`metadata.csv`) that contains the following fields:
    - `station_name`: Name of the radio station (e.g., NPR, BBC Radio 1).
    - `timestamp`: The date and time the recording was captured.
    - `duration`: Recording length in seconds.
    - `filename`: File path for the stored audio file.

### 2.2 Data Splits
- The dataset is provided as a single collection. There is no predefined training/validation/test split since the primary focus is on data collection and analysis.

### 2.3 Sample Data Entry
| station_name  | timestamp           | duration | filename                                  |
|---------------|---------------------|----------|-------------------------------------------|
| Classic FM    | 20250501_143205     | 42       | radio_recordings/Classic_FM_20250501_143205.mp3 |

---

## 3. Data Collection Process

### 3.1 Collection Methodology
- **Automated Script:**  
  An automated Python script was developed using tools such as `ffmpeg`, `pydub`, and `requests`. The script:
  - Randomly selects an online radio station from a predefined list.
  - Records a live audio stream for a duration between 30 to 90 seconds.
  - Saves the recording as an MP3 file.
  - Logs metadata (station name, timestamp, duration, filename) into a CSV file.
  
- **Radio Stations Included:**  
  The list of radio stations includes:
  - NPR, BBC Radio 1, KEXP, Radio Paradise, Jazz24, Classic FM, SomaFM (Groove Salad, Drone Zone), KCRW, and WNYC.
  - These streams are publicly available; however, availability might vary.

### 3.2 Collection Environment
- **Time Period:**  
  March 2025 at IIT Guwahati.
- **Tools & Dependencies:**  
  - Python 3.x, ffmpeg, pydub, pandas, matplotlib.
- **Storage:**  
  Audio files are stored in a designated directory (`radio_recordings`), and metadata is saved as a CSV file in the same directory.

### 3.3 Data Preprocessing and Curation
- **File Naming:**  
  Audio files are named using the station name and a timestamp to ensure uniqueness.
- **Quality Assurance:**  
  The script is designed to ensure exactly 30 successful recordings by retrying any failed attempts.
- **Metadata:**  
  All relevant metadata is systematically documented for each recording.

---

## 4. Dataset Usage

### 4.1 Intended Use
- **Research and Development:**  
  - Audio signal analysis.
  - Multimodal data matching (e.g., aligning audio with silent video clips).
  - Feature extraction and audio classification.
- **Educational Purposes:**  
  - Demonstrations on automated data collection.
  - Laboratory exercises in multimedia data processing.

### 4.2 Potential Misuse
- The dataset is collected from public sources; users must ensure compliance with copyright and licensing terms of the original streams when using or redistributing the dataset.
- The recordings are not intended for commercial broadcasting or redistribution without proper authorization.

---

## 5. Distribution and Licensing

### 5.1 Data Distribution
- The dataset is distributed as:
  - 30 MP3 audio files.
  - A metadata CSV file.
- **Access:**  
  The dataset is intended for academic and research use. It can be shared under the conditions outlined by the creator.

### 5.2 Licensing
- **License Terms:**  
  The dataset is provided under a research license. Redistribution or commercial use may require additional permissions.
- **Attribution:**  
  Users should provide appropriate attribution to the dataset creators and the original radio stations when applicable.

---

## 6. Maintenance and Updates

### 6.1 Versioning
- **Current Version:**  
  This datasheet corresponds to the initial version of the dataset collected in March 2025.
- **Future Updates:**  
  Any corrections, additional recordings, or metadata enhancements will be documented in subsequent versions.

---

## 7. Additional Information

### 7.1 Related Publications or Work
- This dataset is part of the DA323 course project on Multimodal Data Analysis and Learning 2.0.


### 7.2 Limitations
- The dataset is relatively small (30 recordings) and may not cover the full variability of live radio streams.
- Audio quality may vary due to network conditions, stream interruptions, or encoding issues.
- Recordings are limited to the time period and selected radio stations, potentially affecting generalizability.

## 8. Contact Information

For any questions, issues, or further collaboration regarding the RadioStream_Chronicles dataset, please contact:

- **Project Lead:** Rishab Sonthalia
- **Institution:** IIT Guwahati, DA323: Multimodal Data Analysis and Learning 2.0
- **Email:** s.rishab@iitg.ac.in
---

*End of Datasheet*
