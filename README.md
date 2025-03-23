# Sentiment and Emotion Analysis of YouTube Comments: Jake Paul vs. Mike Tyson 🥊

This project analyzes YouTube comments related to Jake Paul and Mike Tyson using natural language processing (NLP) to classify sentiments and detect emotions. The objective is to reveal public opinions and emotional responses toward these figures through data-driven insights.

## 📝 What is Sentiment Analysis?

Sentiment analysis, also known as opinion mining, is the process of evaluating text to determine its emotional tone—categorized as **positive**, **negative**, or **neutral**. Businesses use it to understand customer feedback, and here, we apply it to decode YouTube comments, offering a window into viewer perceptions.

## 🚀 Setup

To replicate this analysis, install the following Python libraries:

- `pandas`: For managing and structuring data
- `numpy`: For numerical computations
- `seaborn`: For advanced data visualization
- `matplotlib`: For creating plots and charts
- `nltk`: For text preprocessing and NLP tasks
- `wordcloud`: For generating visual word clouds

## 🧹 Data Preprocessing
The dataset is cleaned and prepared through these steps:

- Remove Duplicates: Eliminates redundant comments for accurate analysis.
- Handle Missing Values: Drops rows with incomplete data to ensure quality.
- Drop Unnecessary Columns: Removes published_at and author as they’re not relevant.

The processed dataset includes:

- `comment`: The text of each YouTube comment
- `like_count`: Number of likes, reflecting engagement
- `sentiment`: Classified as Positive, Neutral, or Negative
- `emotions`: Detected emotions (e.g., Joy, Anger, Trust)
- Emotion intensity scores: Numeric values for anger, fear, joy, trust, anticipation, surprise, sadness, disgust, positive, and negative

## 📊 Data Analysis and Visualization
The analysis leverages multiple visualization techniques to interpret the data:

### Word Cloud ☁️
A visual representation of frequently used words in comments, where word size indicates frequency. This highlights prominent themes or terms.

### Distribution of Sentiments 📈
A plot showing the proportion of positive, neutral, and negative comments, providing a snapshot of overall sentiment.

### Correlation Heatmap for Emotions 🌡️
A color-coded matrix revealing relationships between emotions. Key observations:

- `anger` and `negative`: Strong correlation (0.79)
- `positive` and `trust`: High correlation (0.81)
- `joy` and `positive`: Strong link (0.80)
- `sadness` and `joy`: Weak correlation (0.28)

### Barplot of Top Emotions 📉
Ranks emotions by their average intensity across comments, identifying the most prevalent feelings.

### Pairplot for Selected Emotions 🔗
A grid of plots showing pairwise relationships between emotions, with kernel density estimations (KDE) on the diagonal. Insights include wider distributions for positive and negative scores, and lower intensity for sadness and anger.

## 💡 Key Insights
- **Sentiment Breakdown**: Uncovers the dominant sentiment among viewers.
- **Emotional Patterns**: Highlights connections, such as the strong tie between positivity and trust.
- **Dominant Emotions**: Identifies which emotions resonate most in the comment dataset.
