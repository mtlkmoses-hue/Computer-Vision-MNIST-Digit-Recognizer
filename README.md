# Computer-Vision-MNIST-Digit-Recognizer
## *A Gentle Introduction to Image Classification*

## Project Overview
This project explores the fundamentals of **Computer Vision** using the famous MNIST (Modified National Institute of Standards and Technology) dataset. The goal is to take a 28x28 grayscale image of a handwritten digit and correctly classify it as a number between 0 and 9.

## Learning Milestones
In this project, I successfully implemented:
- **Data Reconstruction**: Reshaping 1D pixel vectors (784 columns) into 2D images (28x28).
- **Exploratory Data Analysis**: Visualizing class balance to ensure the model wasn't biased toward specific digits.
- **Normalization**: Scaling pixel intensities from [0, 255] to [0, 1] for mathematical stability.
- **Baseline Modeling**: Using **Logistic Regression** to achieve an initial accuracy of ~92%.

## Dataset Structure
- **Features (X)**: 784 pixels representing a flattened 28x28 image.
- **Target (y)**: The digit label (0-9).
- **Training Samples**: 42,000 images.

## Technologies Used
- **Python**
- **Scikit-Learn** (Logistic Regression, Train-Test Split)
- **Matplotlib & Seaborn** (Data Visualization)
- **Pandas & Numpy** (Data Manipulation)

## Key Insights & Results
- **Normalization Matters**: Without scaling the pixels to [0, 1], the model converged much slower and with lower accuracy.
- **Error Analysis**: By inspecting incorrect predictions, I found the model primarily struggles with ambiguous "4s" and "9s" due to their similar geometric shapes.

## How to Run
1. Clone this repository.
2. Download the data from the [Kaggle Digit Recognizer Competition](https://www.kaggle.com/competitions/digit-recognizer).
3. Run the Jupyter Notebook in Google Colab or locally.
