# IndiaWeatherInsights Dataset Datasheet

This document provides a detailed datasheet for the **IndiaWeatherInsights** dataset, a curated collection of weather data for 20 major Indian cities. The dataset is intended for analysis of weather trends and can support various use cases including urban planning, climate research, and data-driven application development.

---

## 1. Dataset Overview

- **Dataset Name:** IndiWeatherInsights  
- **Project:** DA323: Multimodal Data Analysis and Learning 2.0  
- **Version:** 1.0  
- **Date Created:** March 2025  
- **Creators:** Rishab Sonthalia ,IIT Guwahati 
- **Contact:** s.rishab@iitg.ac.in 
- **Description:**  
  IndiaWeatherInsights is a multimodal weather dataset collected using the OpenWeatherMap API. It includes historical and real-time weather data captured periodically over a month, focusing on key meteorological parameters such as temperature, humidity, and wind speed.
- **Primary Creator/Institution:**  
  Assignment-cum-Project-01, DA323: Multimodal Data Analysis and Learning 2.0  
  March 2025, IIT Guwahati
- **Version:** 1.0


---

## 2. Dataset Composition

### Data Instances

Each record in the dataset corresponds to a weather snapshot for one of the 20 Indian cities at a given timestamp. The dataset is stored in CSV format.

### Attributes

- **city**:  
  - *Type:* String  
  - *Description:* Name of the city for which the weather data was collected.
  
- **temperature**:  
  - *Type:* Float (°C)  
  - *Description:* Current temperature in Celsius.
  
- **humidity**:  
  - *Type:* Integer (Percentage)  
  - *Description:* Humidity level expressed as a percentage.
  
- **wind_speed**:  
  - *Type:* Float (m/s)  
  - *Description:* Wind speed in meters per second.
  
- **timestamp**:  
  - *Type:* DateTime  
  - *Description:* Date and time when the data was collected.

### Dataset Size

- **Number of Cities:** 20
- **Collection Frequency:** Data collected periodically (e.g., simulated iterations for demonstration; production usage could span daily/hourly collection over a month).
- **Total Records:** Varies based on the collection period and frequency.

---

## 3. Data Collection Methodology

### Source

- **API:** OpenWeatherMap API  
- **API Endpoint:** `https://api.openweathermap.org/data/2.5/weather`

### Collection Process

- **Automated Collection:**  
  Data is fetched using Python’s `requests` library. For each of the 20 cities, the API is queried with the city name and a valid API key.
  
- **Periodicity:**  
  The dataset simulates periodic data collection over a defined number of iterations (e.g., 5 iterations in a demo setting, scalable to continuous collection over a month).

- **Parameters Captured:**  
  - Temperature
  - Humidity
  - Wind Speed
  - Timestamp of the data capture

- **Tools and Libraries Used:**  
  - Python (`requests`, `pandas`, `matplotlib`)
  - Scheduled or loop-based execution (with `time.sleep` for simulation)

---

## 4. Data Preprocessing and Cleaning

- **Data Format:**  
  Data is stored in CSV format for ease of analysis.
  
- **Preprocessing Steps:**  
  - JSON responses from the API are parsed to extract relevant fields.
  - Data types are standardized (e.g., converting temperature to Celsius, ensuring proper datetime formatting).
  - Error handling is implemented to manage API failures and missing values.

- **Cleaning Procedures:**  
  - Duplicate records (if any) are identified and removed.
  - Timestamps are normalized to ensure chronological order.

---

## 5. Dataset Use Cases

- **Weather Trend Analysis:**  
  Analyze temporal changes in temperature, humidity, and wind speed across different cities.
  
- **Urban Planning and Climate Studies:**  
  Support decisions in urban planning by correlating weather patterns with city infrastructure and environmental planning.
  
- **Machine Learning Models:**  
  Serve as input for predictive models on weather forecasting and anomaly detection.

- **Data Visualization:**  
  Create informative visualizations (e.g., line plots, bar charts) to illustrate weather dynamics over time.

---

## 6. Limitations and Bias

- **Geographical Scope:**  
  The dataset covers only 20 major Indian cities and may not represent weather conditions in rural or less-populated areas.

- **Temporal Resolution:**  
  The frequency of data collection may limit the resolution of short-term weather fluctuations.

- **API Limitations:**  
  Dependence on OpenWeatherMap API means that changes in API terms or outages could affect data consistency.

- **Data Quality:**  
  Weather measurements are subject to sensor errors and reporting delays.

---

## 7. Legal and Ethical Considerations

- **Data Licensing:**  
  The dataset is built using data from OpenWeatherMap, which is subject to their API usage policies. Users must adhere to the OpenWeatherMap terms of service.
  
- **Privacy:**  
  The dataset does not contain any personally identifiable information (PII) and only includes public weather data.

- **Usage Rights:**  
  Users are free to use the dataset for non-commercial or academic purposes, but appropriate credit must be given.

---

## 8. Dataset Maintenance and Updates

- **Update Frequency:**  
  The dataset is designed to be updated periodically (e.g., hourly/daily) over the data collection period. Future updates may include additional parameters or extended geographical coverage.
  
- **Maintenance Plan:**  
  Ongoing maintenance includes:
  - Monitoring API changes or deprecations.
  - Periodic cleaning and validation of collected data.
  - Version control using GitHub for tracking updates and changes.

---

## 9. Contact Information

For any questions, issues, or further collaboration regarding the IndiWeatherInsights dataset, please contact:

- **Project Lead:** Rishab Sonthalia
- **Institution:** IIT Guwahati, DA323: Multimodal Data Analysis and Learning 2.0
- **Email:** s.rishab@iitg.ac.in

---

*This datasheet is intended to provide comprehensive documentation for the IndiWeatherInsights dataset and assist users in understanding its structure, methodology, and potential applications.*
