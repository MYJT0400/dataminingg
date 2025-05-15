# Topic analysis and classification project of fake news and real news

This project uses visualization and machine learning methods to conduct thematic analysis and classification of real and fake news data, including the following:

-Distribution analysis of news topics (bar chart)
-Visualization of Word Cloud in News Headlines
-Extracting Text Features Using TF-IDF
-Using logistic regression for news topic classification

---

## Data Explanation

This project uses the "Fake and Real News Dataset" provided by Kaggle. Two sampled data files were used in the project:

-Sampled_true. csv: Real news samples
-Sampled_fake. csv: Fake News Sample

Please ensure that these two files are in the same directory as the code.

---

## Environmental dependence

Use the following command to install the required libraries:

```bash
pip install pandas matplotlib seaborn wordcloud scikit-learn
```

---

## How to operate

1. **Prepare data files**
Download the 'sampled_true. csv' and 'sampled_fake. csv' files and place them in the directory where the code is located.

2. **Run the script**
The code structure is as follows:

-Load real and fake news data
-Draw a theme distribution map (Seaborn)
-Generate title word cloud map (WordCloud)
-Extract TF-IDF features
-Using logistic regression models to classify news topics
-Output classification report and confusion matrix

---

## Output Content Description

### Visual analysis

-Bar chart of subject distribution for fake news and real news
-News title word cloud, displaying high-frequency keywords

### Model Training and Evaluation

-Training a logistic regression classifier using real news headlines
-Model input: Title
-Model output: Subject category
-Evaluation method:
-Classification report: accuracy, recall, F1 score
-ConfusionMatrixDisplay: Display the classification effect of confusion matrix graphics

---

## Precautions

-By default, only 'sampled_true. csv' is used to train the topic classification model. If you need to merge 'fake_df', you can modify the data loading section yourself.
-If there is an encoding error, you can try reading CSV using 'encoding='utf-8' or 'encoding=ISO-8859-1'.
-To improve the model performance, more complex models such as SVM, Random Forest, etc. can be further used, or data cleaning and preprocessing can be done.

---

## Expansion suggestions

-Attempt to train a model for classifying real and fake news
-Feature extraction and classification of fields outside the title (such as text content)
-Using cross validation to improve model robustness
