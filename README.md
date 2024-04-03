## **Analyzing-Gutenberg-Texts-using-Various-Clustering-Techniques**

### Introduction

Text clustering is a Natural Language Processing (NLP) method used to organize comparable documents or sentences based on their content and meaning. This project explores various methodologies, models, and transformation techniques to cluster documents extracted from five Gutenberg books spanning different genres.

## Dataset

The Gutenberg dataset comprises over 15,000 book texts, with five samples selected for this project, each representing a different genre. The books used in the analysis are:

1. The Mind and the Brain by Alfred Binet (psychology and neuroscience)
2. The Problems of Philosophy by Bertrand Russell (philosophy)
3. The Practice and Science of Drawing by Harold Speed (art)
4. The House on the Borderland by William Hope Hodgson (speculative fiction)
5. Great Pianists on Piano Playing by James Francis Cooke (music)

## Exploratory Data Analysis

This section explores the dataset through various analyses, including:

- Displaying data information
- Calculating character-length for each sentence
- Checking the balance of target classes
- Displaying the top 30 words in clean text
- Visualizing the most frequent 50 words of each book using word clouds

## Data Preparation

The data preparation phase involves creating random samples of 200 documents for each book and preprocessing the data by removing punctuation, digits, non-word characters, extra whitespace, and stop words. Lemmatization is also applied to the words. The resulting dataset is labeled according to the book they belong to for later comparison with clusters.

## Text Transformations

Four text transformation techniques are employed:

1. Bag of Words (BOW)
2. Term Frequency-Inverse Document Frequency (TF-IDF)
3. Word Embedding (Word2Vec)
4. Latent Dirichlet Allocation (LDA)

## Dimensionality Reduction

After text transformation, dimensionality reduction techniques such as Principal Component Analysis (PCA) and t-distributed Stochastic Neighbor Embedding (t-SNE) are applied to visualize the data.

## Models of Clustering

Three clustering algorithms are used:

1. K-Means
2. Expectation Maximization (EM)
3. Hierarchical Clustering (Agglomerative)

Each algorithm is applied with different text transformation techniques, resulting in a total of 12 clustering models.

## Model Evaluation

The clustering models are evaluated using various metrics, including Cohen's kappa, silhouette score, and coherence with LDA. These metrics help assess the effectiveness of the clustering algorithms in capturing the underlying patterns in the data.

## Error Analysis

Error analysis is conducted using the silhouette coefficient to determine the optimal number of clusters. Additionally, pyLDAvis is used to visualize the results of the LDA topic modeling and identify any overlapping or heterogeneous clusters.
