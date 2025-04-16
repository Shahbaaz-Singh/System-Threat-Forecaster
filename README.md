# System-Threat-Forecaster

**System-Threat-Forecaster** is a Machine Learning project designed to predict the probability of a system being infected by various families of malware. The model uses a wide range of telemetry data — including hardware and software features — to make binary classification predictions on system infection risk. This data is originally gathered through antivirus threat reports.

---

## 🚀 Project Background

This project was part of a **private Kaggle-style competition** hosted exclusively for students of the **IIT Madras BS Degree program**. Due to competition privacy policies, we are **not allowed to publicly distribute or upload the original datasets**.

---

## 📁 Dataset Usage Disclaimer

In this repository, there are **three instances of `pd.read_csv(...)`** where dataset files are read. In the original version of the project, these paths referred to the private Kaggle dataset. However:

- **The dataset has been removed** to comply with privacy and competition rules.
- All **Kaggle references have been removed or generalized** to streamline the code for public viewing.
- The repository now serves more as a **project showcase** or template, rather than a ready-to-run script — unless you provide your own dataset.

If you wish to run or extend this project:

> 🔁 **Simply replace the dataset files with your own binary classification dataset**, and adjust preprocessing accordingly.  
The model architecture and core logic can remain largely the same — only the input schema and preprocessing pipeline may need to be tweaked.

---

## 🔧 How to Use

- Plug in your dataset (preferably a binary classification task)
- Update file paths in `pd.read_csv(...)`
- Adjust the preprocessing steps (like encoding or imputation) if necessary
- Run the pipeline to train and evaluate the model

---

## 📄 Note on Evaluation

As part of the original competition, the test labels were hidden and used only on submission to compute accuracy. In the public version in this code part you can just replace the true_labels.csv with your own true labels file.

```python
from sklearn.metrics import accuracy_score

y_test = pd.read_csv("true_labels.csv")['target']
accuracy = accuracy_score(y_test, y_pred)
print(f"Accuracy on test set: {accuracy:.4f}")
```

---

## 🙌 Final Notes

This repository is a **clean, streamlined, and general-purpose version** of my competition project. It's meant to demonstrate skills in:

- Data preprocessing
- Model training & optimization
- Deployment-ready code structure
- Real-world dataset handling under constraints

Feel free to experiment or integrate this pipeline into your own classification problems!

---

Let me know if you want to add a **"Project Structure"** or **"Dependencies/Installation"** section too.
