# BBC news classification

## Basic Setup:
- python3 & pip is required for the project to run
- all the dependencies are listed in `requirements.txt`
- run `pip install -r requirements.txt` to install dependencies

## Usage:
- the python file can be exectued using the command `python3 bbc_classification.py`
- It loads the data in the `/bbc` folder into a pandas dataframe
- During the processing it will open a bunch of graphs in a new window. These need to be closed for the code to proceed.
- There's no other configuration to be done. This is an out of the box model training suite.

## Features:
Data is loaded into a pandas dataframe by traversing the dataset directory, the files need to be present as in the repo for the project to work. The pipeline followed in this project is:

### Data Processing 
- Lower case conversion of text
- Punctuation removal
- Number removal
- Line break removal
- Stop words removal
- Lemmatize text

### Feature Engineering
- TF IDF vectorization
- Word count per text article
- Sentiment Analysis

### Exploratory data analysis
- Input distribution
- Sentiment histogram/density chart
- Word count histogram/density chart
- Word clouds for all categories

### Feature Selection
- SelectKbest chi2

### Model Training & Evaluation
- Train/Test split - 80/20 ratio
- Pipeline to fit & transform all features
- Scaling as & when required for numerical features
- Linear SVC used as classifier with certain params
- Accuracy, Precision, Recall, F1 is scored
- Sample data prediction
>>>>>>> 89bd89805e407919fd41a8b9755a89396da592ca
