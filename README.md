# AlphabetSoup: Predicting Funding Success with Deep Learning

## Project Overview

This project involves using Python and deep learning techniques to create a binary classifier that predicts the success of applicants funded by the nonprofit foundation Alphabet Soup. The analysis is divided into several parts: data preprocessing, neural network modeling, and model optimization.

## Project Structure

### Part 1: Data Preparation
- **Starter_Code.ipynb:** Jupyter notebook for data preprocessing and initial analysis.
  - Load the `charity_data.csv` into a DataFrame.
  - Explore and visualize the dataset to understand its structure and distribution.
  - Use `StandardScaler()` from scikit-learn to normalize the data.
  - Encode categorical variables and split the data into training and testing sets.

### Part 2: Compiling, Training, and Evaluating the Model
- **Starter_Code.ipynb:** Jupyter notebook continuation for neural network modeling.
  - Design and implement a neural network using TensorFlow and Keras.
  - Compile, train, and evaluate the model on the preprocessed data.
  - Save the trained model to an HDF5 file named `AlphabetSoupCharity.h5`.

### Part 3: Optimizing the Model
- **AlphabetSoupCharity_Optimization.ipynb:** Jupyter notebook for model optimization.
  - Apply various optimization techniques to improve model performance.
  - Adjust model parameters, add layers, and use different activation functions.
  - Evaluate the optimized model and save the results to an HDF5 file named `AlphabetSoupCharity_Optimization.h5`.

## Repository Structure

The repository is structured as follows:

- **README.md:** Overview of the project, its structure, and usage instructions.

- **Starter_Code.ipynb:** Jupyter notebook containing Python code for data preprocessing, neural network modeling, and evaluation.

- **AlphabetSoupCharity_Optimization.ipynb:** Jupyter notebook containing Python code for model optimization.

- **Images/:**
  - Contains images used in the final report.

- **AlphabetSoupCharity.h5:** HDF5 file containing the trained model.

- **AlphabetSoupCharity_Optimization.h5:** HDF5 file containing the optimized model.

- **Final Report.md:** Detailed report of the project, including analysis, results, and recommendations.

- **.gitignore:** File to exclude sensitive files and folders like API keys or cache files from version control.

## Tools Used

- Python
- Jupyter Notebook
- Google Colab
- Pandas
- Matplotlib
- Scikit-learn
- TensorFlow
- Keras

## Conclusion

This project demonstrates the application of deep learning techniques to predict the success of funding applicants based on historical data. By following the steps outlined in the Jupyter notebooks, users can preprocess data, build and evaluate a neural network model, and apply various optimization strategies to enhance model performance. Additionally, exploring Random Forests as an alternative approach can provide valuable insights into feature importance and improve prediction accuracy.
