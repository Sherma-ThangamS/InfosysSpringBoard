# Medical Text Analysis and Clustering

This notebook performs an analysis of medical text data, including preprocessing, exploratory data analysis (EDA), and clustering.

## Data Preprocessing

The notebook begins by preprocessing the text data using various techniques:

- **Stop Word Removal:** Removes common English stop words.
- **Stemming:** Reduces words to their root form using Porter Stemmer.
- **Lemmatization:** Reduces words to their base or dictionary form using WordNet Lemmatizer.
- **Spell Checking:** Corrects spelling mistakes using the `autocorrect` library.

## Exploratory Data Analysis (EDA)

EDA is conducted to gain insights into the data. Key features and distributions are visualized, including:

- **Frequent Medical Terms:** Identifies the most common medical terms using word counts.
- **Retained vs. Omitted Words:** Analyzes the words present in the original data and the conversation, comparing the retained and omitted words.
- **Age and Gender Distribution:** Visualizes the distributions of age and gender extracted from the text data.
- **Data Length Analysis:** Shows the distributions of lengths of strings in different columns of the data.
- **Top 50 Frequent words in each column:** Visualizations of the top frequent words in different text columns to understand the patterns.
- **Top 10 Bigrams:** Identifies and visualizes the 10 most frequent two-word combinations in different columns of the data.

## Dashboard

A dashboard with several key visualizations is created using Matplotlib, including:

- Retained vs. Omitted words
- Age Distribution
- Gender Distribution
- Frequent Medical Terms
- Comparison of Retained vs. Omitted Words
- Length distribution of 'data' column
- Length distribution of 'conversation' column
- Top 50 frequent words in 'data' column
- Top 50 frequent words in 'conversation' column


## Model

The notebook utilizes the following techniques to analyze data:

- **TF-IDF Vectorization:** Converts text data into numerical features.
- **K-Means Clustering:** Groups similar medical cases together.
- **t-SNE Visualization:** Visualizes the clusters in a 2D space.
- **PCA dimensionality reduction:** Reduce the dimensions of the feature matrix before clustering to improve performance.


## Symptom Extraction and Analysis

- **Domain-specific NLP model**: Employs a domain-specific NLP model (SciSpaCy) to identify medical terms and symptoms.
- **Symptom Lexicon:** Matches extracted words against a symptom lexicon.
- **TF-IDF vectorization of symptoms**: Creates a TF-IDF representation of extracted symptoms.

## Dependencies

The notebook requires the following libraries:

- `google-colab`
- `pandas`
- `gspread`
- `google-auth`
- `matplotlib`
- `sklearn`
- `seaborn`
- `numpy`
- `nltk`
- `autocorrect`
- `spacy`
- `scispacy`

## Usage

1.  **Install dependencies:** Run the dependency installation commands in the notebook.
2.  **Upload Data:** Upload the required dataset file to Colaboratory.
3.  **Run the notebook:** Execute the cells sequentially to perform data processing, EDA, model training, and visualization.

## Future Improvements

- Expand the symptom lexicon with more medical terms.
- Experiment with different clustering algorithms.
- Evaluate model performance using relevant metrics.
