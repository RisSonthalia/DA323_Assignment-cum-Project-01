# Datasheet for ImageDataset

## 1. Dataset Overview

- **Name:** ImageDataset  
- **Version:** 1.0  
- **Date Created:** March 2025  
- **Creators:** [Rishab Sonthalia / Institution (IIT Guwahati)]  
- **Contact:** [s.rishab@iitg.ac.in]  
- **Description:**  
  This dataset comprises 20 image categories (e.g., Nature, Animals, Cars, etc.), with 50 images per category. Each image is stored as a JPEG file in category-specific folders. A metadata CSV file is provided that documents the source URL, filename, and resolution (width × height) of each image. The dataset is designed for multimodal data analysis and image classification tasks.

## 2. Motivation and Intended Use

- **Purpose:**  
  The dataset was created to facilitate research in scalable image data collection, multimodal analysis, and to serve as a benchmark for image classification models. It can be used to train convolutional neural networks (CNNs) and for tasks such as feature extraction and clustering (using techniques like PCA and t-SNE).

- **Intended Users:**  
  Researchers, data scientists, and developers working in computer vision, machine learning, and multimodal data analysis.

- **Use Cases:**  
  - Training and evaluation of image classification models.
  - Exploratory data analysis and feature extraction.
  - Research on multimodal data matching and analysis.

## 3. Dataset Composition

- **Total Number of Images:**  
  20 categories × 50 images per category = **1,000 images**

- **Data Instances:**  
  Each image instance includes:  
  - The image file in JPEG format.
  - Metadata fields (in a CSV file) including:
    - `category`: The label (e.g., Nature, Animals).
    - `image_url`: The URL from which the image was obtained.
    - `filename`: The saved filename.
    - `resolution`: The dimensions in `width x height` format.

- **Folder Structure:**
 ```
 ImageDataset/
 ├── metadata.csv
 ├── Nature/
 ├── Animals/
 ├── Cars/
 └── ... (other categories)
```


## 4. Data Collection Process

- **Sources:**  
Images were sourced primarily from public image search engines (e.g., Google Images) and potentially other image websites.

- **Methodology:**  
An automated script using Python libraries (e.g., Selenium, Requests, BeautifulSoup) was implemented to:
- Search for images for each of the 20 categories.
- Download 50 images per category.
- Extract metadata (URL, filename, resolution) for documentation.

- **Collection Date:**  
March 2025

- **Curation:**  
The dataset includes only images successfully downloaded and verified via an automated resolution extraction process using the Python Imaging Library (PIL). Images are organized in subfolders corresponding to their categories.

## 5. Preprocessing and Curation

- **Preprocessing Steps:**  
- Automated download and saving of images.
- Extraction of image resolution using PIL.
- Construction of a metadata CSV file to record image details.
- Optional: Image augmentation and resizing for deep learning model training (e.g., via Keras’ ImageDataGenerator).

- **Curation Process:**  
Images that failed to download or did not meet the resolution criteria were excluded. The metadata file was manually reviewed for consistency.

## 6. Legal, Ethical, and Privacy Considerations

- **Copyright:**  
The images are collected from public sources. Users should verify the copyright and usage rights of the original images. The dataset is intended for academic and non-commercial research purposes only.

- **Privacy:**  
The dataset does not contain any personal data or sensitive information.

- **Licensing:**  


- **Ethical Considerations:**  
- Proper attribution should be given when using or referencing images from their original sources.
- Users are encouraged to respect copyright restrictions and use the dataset responsibly.

## 7. Usage Recommendations and Limitations

- **Intended Use:**  
- Image classification and computer vision research.
- Multimodal analysis tasks.
- Educational purposes in academic settings.

- **Limitations:**  
- The dataset size (1,000 images) may be limited for training very large deep learning models.
- Variability in image quality and resolution due to differences in source images.
- Potential bias based on the search terms used and the inherent biases of the image search engine.

- **Recommendations:**  
- Users should consider augmenting the dataset if larger scale experiments are intended.
- Validate image quality and perform additional preprocessing as required for specific research tasks.
- Acknowledge the limitations in any publications or applications that utilize this dataset.

## 8. Maintenance and Future Updates

- **Maintenance:**  
The dataset is maintained by Rishab Sonthalia/ IIT Guwahati. Future updates may include:
- Addition of more categories and images.
- Enhanced metadata (e.g., image annotations, quality scores).
- Updated documentation and user feedback integration.

- **Versioning:**  
Future versions should clearly document changes and updates from previous versions.

- **Contact for Updates/Corrections:**  
For questions, corrections, or suggestions, please contact s.rishab@iitg.ac.in.

## 9. References and Acknowledgements

- **References:**  
- Gebru, T., et al. (2018). "Datasheets for Datasets."  


- **Acknowledgements:**  
- Thanks to the developers of the Python libraries used (Selenium, BeautifulSoup, PIL, etc.).
- Acknowledgment of the public sources of images used in this dataset.

## 10. Additional Notes

- **Documentation Location:**  
This datasheet is included in the dataset repository to ensure transparency and to guide proper usage.

- **Further Work:**  
Users are encouraged to contribute to the dataset, report issues, and suggest improvements via the repository’s issue tracker or contribution guidelines.

## 11. Contact Information

For any questions, issues, or further collaboration regarding the ImageDataset dataset, please contact:

- **Project Lead:** Rishab Sonthalia
- **Institution:** IIT Guwahati, DA323: Multimodal Data Analysis and Learning 2.0
- **Email:** s.rishab@iitg.ac.in

