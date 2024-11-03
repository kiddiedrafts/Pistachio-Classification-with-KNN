# Pistachio Type Classification with K-Nearest Neighbors (KNN)

This project builds a **K-Nearest Neighbors (KNN) classifier** to classify two types of pistachios based on 16 attributes. The dataset used for this project is sourced from Kaggle and contains various features extracted from high-resolution images of pistachios. The goal is to identify the pistachio type based on these features.

## Dataset

The dataset used in this project is sourced from Kaggle and can be found at the following link: [here](https://www.kaggle.com/datasets/belikesaif/16-attribute-pistachio-dataset)

### Dataset Description
- **Class**: The target label indicating the type of pistachio.
- **Features**: 16 distinct attributes describing their area, perimeter, roundness, major and minor axes lengths, eccentricity, solidity, convex area, extent, aspect ratio, roundness, compactness, and various shape factors

### Dataset Location

- **Data/**: This folder will contain the dataset files downloaded from Kaggle.
- **Notebook/**: This folder will house your Jupyter notebooks. **Currently, we are working within the Notebook directory.**


## Project Structure

The main folders and files in the project are structured as follows:

```plaintext
Pistachio/
├── Data/
│   └── [dataset files will be here]             # Dataset CSV file
├── Notebook/
│   └── [your Jupyter notebooks will be here]    # Jupyter notebook with code                 
└── README.md                                    # Project documentation 
```

## Requirements
To run this project, you'll need the following Python libraries:
- `pandas`
- `scikit-learn`


## Feature Engineering and Data Preprocessing
- The data is split into training and testing sets with an 80-20 ratio.
- Standardization is applied to the features in order to normalize the data.

## Model Training
The `k-Nearest Neighbors (k-NN)` algorithm is used to classify the type of pistachios. 
- Cross-validation is performed with different values of `k` to find the best value that gives the highest `F1-score`.
- Once the optimal `k` is determined, a final model is trained on the entire training set.

## Model Performance
The model achieved the following `F1` scores:
- **Training Set F1 Score**: 0.8981
- **Test Set F1 Score**: 0.8372
