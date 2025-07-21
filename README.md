# Twitter-Sentiment-Analysis
Implemented a sentiment analysis model on Twitter reviews to classify them as positive or negative.


# Twitter Sentiment Analysis with TensorFlow

This project implements a sentiment analysis model on real-world Twitter data (from the [Sentiment140 dataset](https://www.kaggle.com/datasets/kazanova/sentiment140)). The model classifies tweets as either **positive** or **negative** using NLP and deep learning techniques (LSTM) in TensorFlow.

---

## 📂 Dataset

- **Source:** [Sentiment140 on Kaggle](https://www.kaggle.com/datasets/kazanova/sentiment140)
- **Size:** 1.6 million tweets
- **Features:**
  - `target`: Sentiment label (0 = Negative, 4 = Positive)
  - `text`: Tweet content
  - Other metadata: `id`, `date`, `user`, etc.

---

##  Model Architecture

- **Text Preprocessing**:
  - Lowercasing, punctuation removal, stopword filtering
  - Tokenization and padding
- **Embedding Layer**: Converts words to dense vectors
- **LSTM Layer**: Captures sequential context in tweet
- **Dropout Layer**: Reduces overfitting
- **Dense Layer**: Binary classification (sigmoid activation)

---

## 📈 Evaluation Metrics

- **Accuracy**
- **Precision / Recall**
- **F1-Score**
- **Confusion Matrix**
- **Training/Validation Loss & Accuracy Curves**

---

## 🧪 Requirements

Install required packages:

```bash
pip install tensorflow pandas numpy seaborn matplotlib scikit-learn nltk kaggle
```
---

## 🚀 How to Run (Google Colab)
Upload kaggle.json for Kaggle access

- Load the dataset using kagglehub

- Preprocess tweets and convert labels

- Build and train the LSTM model

- Evaluate and visualize results
---
## Metrices values 
313/313 ━━━━━━━━━━━━━━━━━━━━ 4s 12ms/step
Classification Report:

                  precision    recall  f1-score   support

           0         0.77      0.74      0.76      4977
           1         0.75      0.78      0.77      5023

    accuracy                              0.76     10000
    macro avg          0.76      0.76     0.76     10000
    weighted avg       0.76      0.76     0.76     10000

---
## Sample Output
Tweet: "I love this product so much!"  
Prediction: Positive ✅

Tweet: "Worst day ever. I'm so done."  
Prediction: Negative ❌

## Further improvement 
Currently the model is misclassifying with some text , we need to tune the hyperparameters or we can also use transformers for better accuracy in few lines of code .
---
## Screenshot

<img width="1189" height="490" alt="TwitterDatavisualization" src="https://github.com/user-attachments/assets/8befe5c4-e942-41c2-9677-981031c7c3d2" />
![ConfusionMatrix](https://github.com/user-attachments/assets/8c7c0a2d-ec34-46ed-a457-3fc71d8f8bb2)


---
✍️ Author
Buddhadeb Bhattacharya
Data Science Enthusiast | AI Intern


