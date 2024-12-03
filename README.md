# SimplyCooking

Team Members: Pascal Reich, Tammy Dahl, Jordan Isaiah Espiritu, Evan Tardiff, Dylan Murphy, Jwann Sy

## Description

Our AI Project is an AI Generated Recommendations for Recipes. Its purpose is to provide a program that can suggests recipes for users based on the ingredients or the type of recipe that is being searched. Based on the selections, the program will
use AI algorithms, such as Word2Vec, K-Mean Clusters, and Cosine Similarity to compare similarity with other recipes and provide more personalized suggestions

## Installation

### Prequisites

This program requires Python 3.10 or later

### Required Packages

Install the necessary libraries using `pip`

```

pip install numpy pandas scikit-learn gensim gradio kaggle
```

### Data Setup

Download the [RecipeNLG Dataset](https://www.kaggle.com/datasets/paultimothymooney/recipenlg) from Kaggle

1. Obtain a Kaggle API token (`kaggle.json`) and set it up

```

mkdir ~/.kaggle

cp path_to_kaggle.json ~/.kaggle/

chmod 600 ~/.kaggle/kaggle.json

``````
  
2. Download the Dataset

```
kaggle datasets download -d paultimothymooney/recipenlg
```

  3. Extract the Dataset

```
unzip recipenlg.zip
```

## Usage

### Google Colab (Recommended)

Run the project effortlessly using Google Colab. Click the button in .ipynb file to launch the notebook

### Local Execution

You can also run the project locally:

1. Clone the repository and navigate to the project folder.

2. Start a Jupyter notebook or execute scripts directly in your IDE.

⚠ **Warning**: Local execution may require significant storage, memory, and computational resources due to the size of the dataset and the training requirements.

## Features

- Ingredient-Based Recommendations: Enter your favorite ingredients to discover matching recipes.

- Recipe ID Recommendations: Use a specific recipe ID to find similar dishes.

- Cluster Recommendations: Explore recipes within the same category.

## Training the Model

Train the recommendation system using the following steps:

1. Load and preprocess the RecipeNLG dataset.

2. Train a Word2Vec model on the cleaned ingredient lists.

3. Generate recipe vectors and cluster them using K-means.

4. Save the trained models for inference.

## Testing and Frontend
  

### Interactive CLI

Run the CLI cell to interact with the system via command line.


### Web Interface (Gradio)

Launch the Gradio cell for a user-friendly experience.


