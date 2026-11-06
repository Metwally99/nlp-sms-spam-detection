# SMS Spam Detection with NLP

An exploratory machine-learning notebook that cleans text, engineers features, and compares classifiers for spam detection.

## What the notebook covers

- Explores label balance and message characteristics.
- Preprocesses text with regular expressions, stop-word removal, and lemmatization.
- Builds TF-IDF features and explores Naive Bayes, decision trees, and random forests.
- Uses classification reports and confusion matrices to inspect predictions.

**Tools:** Python, pandas, NumPy, NLTK, scikit-learn, Matplotlib, and seaborn. The notebook also contains TensorFlow/Keras experimentation.

## Repository

| File | Purpose |
| --- | --- |
| [Code.ipynb](Code.ipynb) | Data exploration, feature preparation, and model experiments |

## Running the notebook

1. Create a Python environment and install the dependencies:

   ```bash
   pip install jupyter numpy pandas matplotlib seaborn nltk scikit-learn tensorflow
   ```

2. Make the dataset available locally. The notebook references `combined_enron.csv` and another CSV through absolute paths that are specific to the original environment. Update those paths to match your files. **The datasets are not included in this repository.**
3. Open `Code.ipynb` in Jupyter or an editor that supports notebooks. Install any required NLTK resources when prompted, then run the cells in order.

## Evaluation notes

The current notebook performs parts of preprocessing and balancing before the train/test split. This can introduce data leakage, so the saved scores should be treated as exploratory. A stronger evaluation would split first, fit text transformations and resampling on training data only, and evaluate on an untouched test set.

## Next improvements

- Replace absolute file paths with configurable paths.
- Package preprocessing and model training in a reproducible pipeline.
- Report precision, recall, F1, and a confusion matrix on held-out data.
