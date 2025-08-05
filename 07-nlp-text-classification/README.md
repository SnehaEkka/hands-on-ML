# Text Classification on AI-Generated Abstracts

## Objective

This exercise explores supervised text classification using a dataset of academic abstracts, with the core goal of distinguishing between AI-generated and human-written content. Students will build, evaluate, and interpret models that can reliably classify abstracts from the **AI-GA (Artificial Intelligence Generated Abstracts) dataset**.

**Dataset:** The dataset contains 14,331 academic abstracts (7,248 AI-generated via GPT-3, 7,082 original), with fields for abstract text, title, and label (0 = original, 1 = AI-generated).

## Skills Demonstrated

- Text preprocessing, tokenization, and feature extraction for natural language data
- Application of machine learning algorithms for document classification
- Use of cross-validation and relevant performance metrics
- Interpretation of model outputs and feature importances
- Visualization and communication of findings

## Tools Used

- Python (pandas, numpy, nltk, scikit-learn, spaCy)
- Jupyter Notebook for analysis, model building, and visualization

## Summary of Work

- Loaded and inspected the AI-GA dataset, verifying sample counts and target label distribution.
- Performed essential text preprocessing steps: lowercasing, tokenization, stopword removal, and lemmatization to clean and normalize the abstract text.
- Engineered document-term matrices and other relevant features.
- Developed and compared machine learning models (e.g., logistic regression, SVM, or tree-based models) for classifying abstracts.
- Employed cross-validation to assess generalization, reporting metrics such as accuracy, precision, recall, F1-score, and confusion matrices.
- Analyzed which words or n-grams most strongly influence predictions through model interpretability tools.
- Visualized results and model diagnostics to support analytical conclusions.

## Key Findings

The best-performing classifiers achieved high accuracy in distinguishing AI-generated from original abstracts, with cross-validated accuracy often exceeding 92%. Feature analysis revealed distinctive vocabulary and structural differences leveraged by the models, such as the prevalence of generic language and phrasings in AI-generated abstracts. Precision and recall balanced across labels, and the confusion matrix showed robust discrimination with minimal misclassification.

These results demonstrate that, although advanced, AI-generated text retains subtle statistical signatures that well-tuned algorithms can detect, highlighting both the opportunities and limits of automated text generation in scholarly contexts.

## Course Context

Completed as part of the Boston University MSBA program: Unsupervised Machine Learning course (BA820) in the module on text mining and NLP.
