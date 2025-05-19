**📊 Sentiment Analysis: Model Comparison**

**Author: Deekshitha Chowdary Kalluri**

**Course: CIS 732 – Machine Learning (Term Project)**

**📂 Included Files**

- SentimentClassification.ipynb — Jupyter notebook for model training, evaluation, and visualization

- FINAL REPORT.pdf — Detailed report with methodology, results, and analysis

- FINAL PPT.pptx — Summary presentation slides

- IMDB Dataset.csv — Preprocessed, balanced IMDb movie review dataset (2,500 samples)

- README.md — Project overview and submission details

**📝 Project Summary**

This project evaluates and compares the performance of four sentiment classification models on a curated IMDb movie review dataset:

- Logistic Regression

- Linear Support Vector Classifier (LinearSVC)

- Long Short-Term Memory (LSTM)

- BERT (Bidirectional Encoder Representations from Transformers)


All models were trained on binary-labeled data (positive vs. negative), with standardized preprocessing and evaluation using:

- Accuracy

- F1 Score

- AUC-ROC

- Confusion Matrix


**🔍 Key Findings**
**✅ Classical Models**

- Logistic Regression

  - Accuracy: 0.842

  - F1 Score: 0.8448

  - AUC-ROC: 0.9256

- LinearSVC

  - Accuracy: 0.850

  - F1 Score: 0.8497

  - AUC-ROC: 0.9254

  - Performed best among classical methods


**🔁 LSTM Model**

- Struggled due to limited data and vocabulary

- Accuracy: 0.50, F1 Score: 0.0602

- Severe underfitting observed


**🤖 Transformer Model (BERT)**

- Pretrained BERT (no fine-tuning)

  - Accuracy: 0.496, F1 Score: 0.6471

  - Poor balance in classification

- Fine-Tuned BERT

  - Accuracy: 0.932, F1 Score: 0.9308, AUC-ROC: 0.977

  - Outperformed all other models


**📈 Statistical Analysis**

Paired t-tests were conducted comparing fine-tuned BERT against baseline models. While BERT achieved the best metrics, no statistically significant differences were found due to sample size limitations.


**📌 Conclusion**

- LinearSVC is a strong classical baseline for small datasets

- Fine-tuned BERT achieves the best overall performance

- LSTM and unfine-tuned BERT models underperformed in this scenario

- Statistical validation is critical when working with small datasets


**🔮 Future Work**

- Use larger datasets

- Experiment with RoBERTa, DistilBERT, or LoRA adapters

- Tune hyperparameters and training epochs

- Explore prompt engineering for transformer models


**🔗 Project Repository: https://github.com/DeekshithaKalluri/SentimentAnalysis**
