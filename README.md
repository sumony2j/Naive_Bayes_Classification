# Naive Bayes Classification

## Introduction

Naive Bayes classification is a probabilistic machine learning algorithm used for classification tasks. It is based on Bayes' theorem, which describes the probability of an event based on prior knowledge of conditions related to the event. Despite its simplicity, Naive Bayes classifiers often perform well in practice and are widely used in various applications. This repository provides an overview of Naive Bayes classification along with examples and implementations in Python.


## How Naive Bayes Classification Works

Naive Bayes classification works by computing the probability of each class label given the input features and selecting the class with the highest probability. It makes the "naive" assumption that the features are conditionally independent given the class label, which simplifies the computation of probabilities.

### Bayes' Theorem:

P(y|X) = ( P(X|y) * P(y) ) / P(X)


### Model Training:
1. **Calculate Class Priors**: Estimate the prior probability of each class based on the frequency of class labels in the training data.
2. **Calculate Class Conditional Probabilities**: Estimate the conditional probability of each feature given each class label.
3. **Predictions**: Given new input features, calculate the posterior probability of each class using Bayes' theorem and select the class with the highest probability.

## Types of Naive Bayes Classifiers

- **Gaussian Naive Bayes**: Assumes that continuous features follow a Gaussian (normal) distribution.
- **Multinomial Naive Bayes**: Suitable for features that represent counts or frequencies (e.g., word counts in text classification).
- **Bernoulli Naive Bayes**: Applicable when features are binary variables (e.g., presence or absence of a word in text).

## Advantages of Naive Bayes Classification

- Simple and easy to understand.
- Efficient and computationally inexpensive to train.
- Performs well in practice, especially for text classification and other high-dimensional datasets.
- Handles both continuous and discrete features.

## Limitations of Naive Bayes Classification

- Assumes independence between features, which may not hold true in real-world datasets.
- Sensitivity to the quality of input features and the presence of irrelevant or correlated features.
- Cannot capture complex relationships between features.

## Applications of Naive Bayes Classification

- Text classification and sentiment analysis.
- Email spam detection.
- Medical diagnosis and disease prediction.
- Recommendation systems.
- Customer churn prediction in marketing.

## Datasets

This repository includes sample datasets in CSV format that can be used to practice Naive Bayes classification. The datasets contain features relevant to classification tasks.

##  Repository Structure

```sh
└── Naive_Bayes_Classification/
    ├── Dataset_Details.md
    ├── Naive_Bayes.ipynb
    ├── README.md
    ├── mushrooms.csv
    └── requirements.txt
```

##  Getting Started

***Requirements***

Ensure you have the following dependencies installed on your system:

* **JupyterNotebook**

###  Installation

1. Clone the Naive_Bayes_Classification repository:

```sh
git clone https://github.com/sumony2j/Naive_Bayes_Classification.git
```

2. Change to the project directory:

```sh
cd Naive_Bayes_Classification
```

3. Install the dependencies:

```sh
pip install -r requirements.txt
```

###  Running Naive_Bayes_Classification

Use the following command to run Naive_Bayes_Classification:

```sh
jupyter nbconvert --execute notebook.ipynb
```

##  Contributing

Contributions are welcome! Here are several ways you can contribute:

- **[Submit Pull Requests](https://github.com/sumony2j/Naive_Bayes_Classification.git/blob/main/CONTRIBUTING.md)**: Review open PRs, and submit your own PRs.
- **[Join the Discussions](https://github.com/sumony2j/Naive_Bayes_Classification.git/discussions)**: Share your insights, provide feedback, or ask questions.
- **[Report Issues](https://github.com/sumony2j/Naive_Bayes_Classification.git/issues)**: Submit bugs found or log feature requests for Naive_bayes_classification.

<details closed>
    <summary>Contributing Guidelines</summary>

1. **Fork the Repository**: Start by forking the project repository to your GitHub account.
2. **Clone Locally**: Clone the forked repository to your local machine using a Git client.
   ```sh
   git clone https://github.com/sumony2j/Naive_Bayes_Classification.git
   ```
3. **Create a New Branch**: Always work on a new branch, giving it a descriptive name.
   ```sh
   git checkout -b new-feature-x
   ```
4. **Make Your Changes**: Develop and test your changes locally.
5. **Commit Your Changes**: Commit with a clear message describing your updates.
   ```sh
   git commit -m 'Implemented new feature x.'
   ```
6. **Push to GitHub**: Push the changes to your forked repository.
   ```sh
   git push origin new-feature-x
   ```
7. **Submit a Pull Request**: Create a PR against the original project repository. Clearly describe the changes and their motivations.

Once your PR is reviewed and approved, it will be merged into the main branch.

</details>
