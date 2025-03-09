# Datasheet for the Multimodal National Symbols Dataset

## 1. Dataset Overview

- **Dataset Name:** Multimodal National Symbols Dataset  
- **Project:** DA323: Multimodal Data Analysis and Learning 2.0  
- **Version:** 1.0  
- **Date Created:** March 2025  
- **Creators:** Rishab Sonthalia ,IIT Guwahati 
- **Contact:** s.rishab@iitg.ac.in 

### 1.1 Purpose
- To facilitate research in multimodal data analysis by providing a dataset that integrates visual, textual, and audio modalities related to national symbols.
- To enable studies on the correlations between flag designs, anthem texts, and anthem audio, and support tasks such as cross-modal generation (e.g., generating anthem text from flag features).

### 1.2 Intended Uses
- Multimodal feature extraction and correlation analysis.
- Cross-modal generation research (e.g., mapping from flag images to anthem text or audio features).
- Educational purposes in data collection, preprocessing, and multimodal machine learning.

### 1.3 Unintended Uses
- Not intended for political or cultural profiling beyond academic research.
- Should not be used to support political propaganda or biased cultural assessments.

## 2. Composition

### 2.1 Modalities Included
- **Flags:**  
  High-quality PNG images representing the national flags of at least 100 countries.  
  - **Format:** PNG images with filenames corresponding to two-letter country codes.
  
- **Anthem Text:**  
  English translations of national anthems corresponding to the flags.  
  - **Format:** JSON file (`anthem_translations.json`) mapping country codes to anthem text.
  
- **Anthem Audio:**  
  MP3 files of national anthems for a subset of countries.  
  - **Format:** MP3 files stored in a designated folder (e.g., `anthem_mp3/`) with filenames based on country codes.

### 2.2 Data Instances
- **Number of Samples:**
  - Approximately 230 flag images.
  - Anthem text for the same set of nations.
  - Anthem audio files for a subset of those nations.
- **Annotations:**
  - Flag images: Implicitly annotated via country codes.
  - Anthem text: Unannotated, raw translations.
  - Anthem audio: Raw audio recordings.

## 3. Collection Process

### 3.1 Data Sources
- **Flags:**  
  Downloaded from public repositories (e.g., via the `svg-country-flags` package on GitHub) and converted to PNG.
  
- **Anthem Text & Audio:**  
  Sourced from [nationalanthems.info](https://nationalanthems.info/) using automated scraping methods.

### 3.2 Data Collection Methods
- **Flags:**  
  Collected using npm commands and GitHub repositories.
- **Anthem Text & Audio:**  
  Scraped programmatically, with URLs constructed based on country codes.

### 3.3 Data Curation and Preprocessing
- **Flags:**  
  Processed using a CNN (e.g., VGG16) to extract high-dimensional features such as color distributions and aspect ratios.
- **Anthem Text:**  
  Preprocessed by lowercasing, punctuation removal, and stop word filtering; features extracted using TF-IDF (with or without dimensionality reduction).
- **Anthem Audio:**  
  Audio features (e.g., tempo, MFCCs, spectral features) extracted using Librosa.

### 3.4 Ethical Considerations
- Data is collected from publicly available sources.
- Adherence to the terms of use of source websites.
- No personally identifiable or sensitive information is included.

## 4. Preprocessing and Cleaning

- **Flags:**  
  Standard image preprocessing (resizing, normalization) applied; CNN-based feature extraction to derive detailed visual descriptors.
- **Anthem Text:**  
  Text cleaning (lowercasing, removal of non-alphabetic characters) and TF-IDF feature extraction.
- **Anthem Audio:**  
  Audio processing using standard libraries (e.g., Librosa) to extract tempo, MFCCs, and other audio descriptors.
- Quality checks were performed to ensure consistency and alignment across modalities.

## 5. Uses

### 5.1 Potential Applications
- **Multimodal Analysis:**  
  Correlating visual, textual, and audio features to study cultural, historical, and aesthetic patterns.
- **Cross-Modal Generation:**  
  Building models that can generate anthem text or audio themes from flag images, and vice versa.
- **Educational Tools:**  
  Serving as a comprehensive dataset for teaching data collection, preprocessing, and multimodal machine learning.

### 5.2 Limitations and Biases
- **Data Coverage:**  
  Limited by the availability and quality of public sources.
- **Cultural Bias:**  
  Anthem translations and flag designs may reflect cultural or historical biases.
- **Modality Alignment:**  
  Inconsistencies between modalities (e.g., missing anthem audio for some countries) may affect analysis.

## 6. Distribution and Maintenance

### 6.1 Licensing and Access
- Intended for academic and research use.
- Users must adhere to the licensing terms of the original data sources.
- Proper citation of source materials is required.

### 6.2 Data Maintenance
- The dataset will be maintained in a public repository (e.g., GitHub).
- Future updates may include additional countries, refined annotations, or improved preprocessing methods.


## 7. Contact Information

For any questions, issues, or further collaboration regarding the Multimodal National Symbols Dataset , please contact:

- **Project Lead:** Rishab Sonthalia
- **Institution:** IIT Guwahati, DA323: Multimodal Data Analysis and Learning 2.0
- **Email:** s.rishab@iitg.ac.in

---

*This datasheet provides a formal overview of the Multimodal National Symbols Dataset, integrating flag images, anthem translations, and anthem audio. It is intended to support research and educational initiatives in multimodal analysis and generative modeling.*
