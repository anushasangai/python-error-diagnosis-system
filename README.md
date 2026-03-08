# Retrieval-Based Python Error Diagnosis System

This project builds a retrieval-based system that helps diagnose Python runtime errors by finding similar past errors.

Instead of training a classifier, the system converts error messages into numerical vectors and retrieves the most similar errors using cosine similarity.

## Project Pipeline

Python Error
↓
Text Cleaning
↓
TF-IDF Vectorization
↓
Cosine Similarity
↓
Top-3 Similar Errors
↓
Root Cause + Suggested Fix

## Technologies Used

* Python
* Pandas
* Scikit-learn
* TF-IDF Vectorization
* Cosine Similarity

## Dataset

The dataset contains common Python runtime errors along with their root causes and suggested fixes.

Columns in the dataset:

* traceback
* root_cause
* fix

## Example

Input Error:

TypeError: can only concatenate str to int

Output:

Similar Error: TypeError unsupported operand type for + int and str
Root Cause: Trying to add integer and string
Suggested Fix: Convert string to integer before addition

## How to Run

1. Clone the repository
2. Open the notebook `error_diagnosis.ipynb`
3. Run the cells sequentially
4. Use the `diagnose_error()` function to test new errors

## Conclusion

This project demonstrates how information retrieval techniques can assist developers in debugging Python runtime errors by leveraging text similarity and vector representations.
# python-error-diagnosis-system
Retrieval-based system that diagnoses Python runtime errors using TF-IDF and cosine similarity.
