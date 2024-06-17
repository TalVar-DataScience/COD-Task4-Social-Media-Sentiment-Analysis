NAME: TALLURI VARUN
ID: CT08DS1001
DOMAIN: DATA ANALYTICS
DURATION: 20th MAY 2024 to 20th JUNE 2024
MENTOR: SRAVANI GOUNI
DESCRIPTION:
Social media sentiment analysis involves extracting, processing, and analyzing textual data from social media platforms to determine the sentiment expressed by users. This task leverages various data processing and natural language processing techniques to achieve this goal. The dataset used in this task contains social media posts with associated sentiment labels, making it suitable for sentiment analysis.

By completing this Task of Social Media Sentiment Analysis, the following are the objectives that I have achieved:

- Understanding the Data: I have gained a comprehensive understanding of the dataset's structure, variables, and types of data.
- Data Cleaning: I have identified and handled noisy data by removing irrelevant components such as URLs, mentions, hashtags and numbers.
- Text Preprocessing: I have tokenized the text, removed non-alphanumeric characters, and filtered out stopwords to prepare the text for analysis.
- Sentiment Analysis: I have used the VADER sentiment analysis tool to assign sentiment scores to the cleaned text.
- Data Visualization: I have visualized the distribution of sentiment scores to understand the overall sentiment expressed in the social media posts.


The following are the steps that I have followed for doing the Task:

Loading the Data

- I have loaded the social media dataset using pandas.
- Column names were specified to ensure correct parsing of the dataset, and encoding was set to 'latin1' to handle special characters present in the text data.
- The first few rows were displayed to understand the structure of the dataset.

Data Preprocessing

Cleaning Text Data:
  - URLs, mentions, hashtags, and numbers were removed using regular expressions.
  - Text was converted to lowercase to ensure uniformity.
  - Tokenization was performed to split the text into individual words.
  - Non-alphanumeric tokens were removed to clean the text further.
  - Stopwords (commonly used words that do not contribute to the sentiment) were removed using NLTK's stopwords list.
  - The cleaned text was stored in a new column called 'cleaned_text'.
  
Limiting Data for Demonstration:
  - To make the process manageable and to ensure quick execution, the dataset was limited to the first 1000 rows.

Sentiment Analysis

Sentiment Scoring:
  - The VADER SentimentIntensityAnalyzer was used to compute sentiment scores for the cleaned text.
  - The compound sentiment score, representing the overall sentiment of the text, was extracted and stored in a new column called 'sentiment'.


Data Visualization

Sentiment Distribution:
  - A histogram was plotted to visualize the distribution of sentiment scores across the dataset.
  
Time Series Visualization:
  - If the dataset contained a 'timestamp' column, sentiment scores were aggregated over time to observe trends.
  - This involved converting the 'timestamp' column to datetime format, setting it as the index, resampling the data by month, and plotting the average sentiment score over time.

Handling Missing Columns

- The presence of the 'text' column was checked before proceeding with text processing and sentiment analysis. If absent, an appropriate message was printed.


CONCLUSION:

Through this process of social media sentiment analysis, I was able to:

- Load and inspect the social media dataset.
- Clean and preprocess the text data to remove noise and irrelevant components.
- Apply sentiment analysis using the VADER tool to assign sentiment scores to the text.
- Visualize the distribution of sentiment scores using a histogram.
- Visualize sentiment trends over time if a timestamp was available.

These steps have provided a comprehensive framework for understanding and analyzing sentiment expressed in social media posts. The insights gained from this analysis can be valuable for businesses, researchers and policymakers to make informed decisions based on public sentiment.
