# US-Politician-Tweet-Analysis
Certainly! Below is a detailed and professional `README.md` file tailored to your project, which focuses on analyzing the tweets of politicians before and after elections. This README provides an in-depth overview of the project, its objectives, methodology, and outputs. It also acknowledges contributors and includes instructions for using the provided files.

---

# Political Tweets Analysis

## Overview

This project focuses on analyzing the tweets of prominent U.S. politicians to uncover trends, sentiment patterns, and linguistic characteristics before and after major election periods. The analysis aims to provide insights into how political messaging evolves during critical times in the electoral cycle. 

The dataset includes tweets from:
- **Donald Trump**
- **Alexandria Ocasio-Cortez**
- **Bernie Sanders**
- **Josh Hawley**
- **Ron DeSantis**
- **Elizabeth Warren**

The cleaned and processed data has been used to create an interactive **Power BI dashboard** that visualizes tweet frequency, sentiment distribution, word clouds, and other key metrics. This repository also includes the final cleaned dataset (`All_politicians_cleaned_tweets_final.xlsx`) for further exploration or integration into other tools.

---

## Project Objectives

1. **Data Cleaning**: Standardize and preprocess raw tweet datasets to ensure consistency and usability.
2. **Sentiment Analysis**: Analyze the sentiment of tweets (positive, negative, neutral) to understand emotional tone.
3. **Temporal Analysis**: Compare tweet activity and sentiment before and after election periods.
4. **Linguistic Insights**: Extract key nouns and phrases to identify recurring themes in political discourse.
5. **Visualization**: Create an interactive Power BI dashboard to present findings in an accessible and engaging format.

---

## Key Deliverables

### 1. **Final Cleaned Dataset**
- File: `All_politicians_cleaned_tweets_final.xlsx`
- Description:
  - A unified dataset containing cleaned tweets from all politicians.
  - Columns include: `Date`, `Tweet`, `Politician_name`, `Year`, `Month`, `Day`, `Weekday`, `Nouns`, `Sentiment`, and `Sentiment_Category`.
  - This dataset can be used for further analysis or integrated into visualization tools like Tableau, Excel, or Power BI.

### 2. **Power BI Dashboard**
- File: `Tweet_analysis_dashboard.pbix`
- Description:
  - An interactive dashboard showcasing:
    - Tweet frequency over time.
    - Sentiment distribution by politician.
    - Word clouds highlighting frequently used terms.
    - Comparison of tweet sentiment before and after election periods.
  - Instructions for use are provided below.

---

## Methodology

### 1. Data Collection
- Raw tweet datasets were collected for each politician across multiple years.
- Datasets included metadata such as date, tweet content, and engagement metrics (likes, retweets, etc.).

### 2. Data Cleaning and Preprocessing
- **Standardization**:
  - Removed unnecessary columns (e.g., image links, video thumbnails).
  - Renamed columns for consistency (e.g., `Content` → `Tweet`).
  - Split tweets separated by line breaks into individual rows.
- **Date Formatting**:
  - Extracted and standardized dates to `YYYY-MM-DD` format.
  - Removed timezone information and ordinal suffixes (e.g., "1st", "2nd").
- **Text Cleaning**:
  - Removed URLs, special characters, and converted text to lowercase.
  - Applied SpaCy's natural language processing (NLP) pipeline to extract nouns and proper nouns.
- **Null Handling**:
  - Dropped rows with missing values to ensure data quality.

### 3. Feature Engineering
- **Sentiment Analysis**:
  - Used `TextBlob` to calculate sentiment polarity for each tweet.
  - Categorized tweets as `Positive`, `Negative`, or `Neutral`.
- **Temporal Features**:
  - Extracted year, month, day, and weekday from the `Date` column.
- **Election Periods**:
  - Tagged tweets as occurring `Before` or `After` specific election dates.

### 4. Advanced Analysis
- **TF-IDF Vectorization**:
  - Identified unique keywords associated with each politician using TF-IDF scores.
- **Cosine Similarity**:
  - Calculated similarity between politicians based on their tweet content.
- **Word Clouds**:
  - Generated word clouds to visualize the most common words across all tweets.

### 5. Visualization
- Created an interactive Power BI dashboard to present key findings in an intuitive and visually appealing manner.

---

## How to Use This Repository

### 1. Download the Files
- Clone this repository or download the following files directly:
  - `All_politicians_cleaned_tweets_final.xlsx`: Final cleaned dataset.
  - `Tweet_analysis_dashboard.pbix`: Power BI dashboard.

### 2. Explore the Dataset
- Open `All_politicians_cleaned_tweets_final.xlsx` to analyze the cleaned data.
- Use Python, Excel, or other tools to perform custom analyses.

### 3. Use the Power BI Dashboard
- Open the `Tweet_analysis_dashboard.pbix` file in Power BI Desktop.
- Interact with the visualizations to explore tweet trends, sentiment, and linguistic patterns.

### 4. Reproduce the Analysis
- Install the required Python libraries by running:
  ```bash
  pip install pandas spacy textblob matplotlib seaborn wordcloud scikit-learn
  ```
- Follow the steps outlined in the PDF (`Data_cleaning-Copy1.pdf`) to reproduce the cleaning and analysis pipeline.

---

## Contributions

This project was made possible through the efforts of:

- **Chaitanya Vinay Sure**: Contributed to data cleaning, preprocessing, and analysis.

If you find any issues with the project or have suggestions for improvement, feel free to open an issue or submit a pull request.

---

## License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute the content as per the terms of the license.

---

"# US-Politician-Tweet-Analysis" 
