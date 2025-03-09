# IITG_MultimodalTextDataset Datasheet

## 1. Overview
- **Dataset Name:** IITG_MultimodalTextDataset  
- **Project:** DA323: Multimodal Data Analysis and Learning 2.0  
- **Version:** 1.0  
- **Date Created:** March 2025  
- **Creators:** Rishab Sonthalia ,IIT Guwahati 
- **Contact:** s.rishab@iitg.ac.in  
- **Description:**  
  This dataset contains text data collected across 20 distinct categories. The text is extracted from multiple websites using automated crawling techniques and then preprocessed using Natural Language Processing (NLP) methods. The dataset is intended for educational purposes, demonstrating tasks such as text classification, sentiment analysis, topic modeling, and exploratory data analysis (EDA).

- **Modality:** Text

## 2. Data Collection Methodology
- **Source Selection:**  
  For each category, three websites were chosen based on relevance and availability of textual content. The categories include Technology, Sports, Health, Politics, Entertainment, Business, Science, Education, Environment, Travel, Food, Fashion, Art & Culture, Finance, History, Literature, Music, Gaming, Lifestyle, and World News.

- **Crawling Approach:**  
  - Tools: Python libraries (`requests`, `BeautifulSoup`, and `Scrapy` where applicable).
  - Process:  
    1. Send HTTP GET requests to each website.
    2. Parse the HTML with BeautifulSoup.
    3. Extract the title, publication date (if available), and text content (by targeting `<article>` or `<p>` tags).
  - **Storage:**  
    - Raw text data for each category is saved into separate files.
    - Preprocessed (cleaned) text is stored in a separate folder.

## 3. Data Preprocessing
- **Cleaning Steps:**  
  1. Removal of residual HTML tags using BeautifulSoup.  
  2. Conversion of all text to lowercase.  
  3. Removal of punctuation, including standard punctuation and additional typographic characters (e.g., “ ”, ‘ ’, —, –).  
  4. Tokenization using NLTK's `word_tokenize`.  
  5. Removal of English stop words using NLTK's stop words list.

- **Outcome:**  
  The data is available in two forms:  
  - **Raw Data:** Directly extracted from the source without modification.  
  - **Cleaned Data:** Processed text stored separately in a structured folder.

## 4. Data Statistics
- **Total Categories:** 20  
- **Samples:**  
  Each category file currently provides one sample (one aggregated text per category).  
  - **Total Samples:** 20 (one per category)
  
- **Label Distribution:**  
  Due to the dataset size, each category has exactly one sample, which presents limitations for training robust models.

## 5. Limitations and Considerations
- **Sample Size:**  
  The dataset contains only one sample per category, making it unsuitable for training high-capacity models without further data augmentation.
- **Dynamic Content:**  
  Some websites may load content dynamically (via JavaScript) and the current crawling method might not capture the full text.
- **Preprocessing Impact:**  
  Aggressive cleaning (e.g., removal of punctuation) may remove useful tokens; adjustments may be necessary depending on the analysis.
- **Usage:**  
  Intended primarily for educational and exploratory analysis. For production-level applications, more extensive data collection is required.

## 6. Potential Use Cases
- **Text Classification:** Demonstrating a pipeline for classifying text by category.
- **Topic Modeling:** Using methods such as LDA to uncover latent topics.
- **Sentiment Analysis:** Analyzing the sentiment distribution across different categories.
- **Exploratory Data Analysis (EDA):** Visualizations (word clouds, frequency distributions, n-gram analysis).
- **Multimodal Analysis:** Serving as a textual component in a broader multimodal dataset.

## 7. File Structure
- **Raw Data Folder:** `text_dataset/raw/`  
  Contains raw text files named by category (e.g., `Technology.txt`).

- **Cleaned Data Folder:** `text_dataset/cleaned/`  
  Contains preprocessed text files named by category (e.g., `Technology.txt`).

## 8. Dataset Creation Pipeline
- **Web Crawling:** Extract text from selected websites per category.
- **Preprocessing:** Clean the text using the custom pipeline described above.
- **Storage:** Save both raw and cleaned data into dedicated directories.
- **Analysis:** The dataset is further used for various analyses (n-gram analysis, sentiment analysis, topic modeling, and classification).




## 9. Contact Information

For any questions, issues, or further collaboration regarding the IITG_MultimodalTextDataset dataset, please contact:

- **Project Lead:** Rishab Sonthalia
- **Institution:** IIT Guwahati, DA323: Multimodal Data Analysis and Learning 2.0
- **Email:** s.rishab@iitg.ac.in

---

This datasheet provides a detailed overview and formal documentation of the IITG_MultimodalTextDataset, covering its creation, preprocessing, contents, and limitations. Adjust the details as needed based on the actual data and project outcomes.
