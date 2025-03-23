# Spine Condition Analysis using Machine Learning

## **Project Overview**
This project applies machine learning models to analyze **biomechanical data** and predict **lower back pain** conditions. By identifying critical spinal features, we aim to improve the diagnosis and prediction of abnormalities in spine health.

## **Objective**
- Use **ML models** on biomechanical data to predict lower back pain.
- Identify spinal features that most contribute to lower back pain.
- Explore feature importance to enhance prediction accuracy.

## **Dataset Overview**
**Dataset**
The dataset used in this project is stored in the `dataset/` folder.

🔗 [Download Dataset](https://github.com/jadavbindupriya/Spinal_Condition_Analysis/blob/main/dataset/Dataset_spine.csv)

- **Features:**
  - Pelvic Incidence, Pelvic Tilt, Lumbar Lordosis Angle, Sacral Slope, Pelvic Radius
  - Degree Spondylolisthesis, Pelvic Slope, Direct Tilt, Thoracic Slope, Cervical Tilt, Sacrum Angle, Scoliosis Slope
- **Target Variable:** Normal/Abnormal (Binary Classification)
- **Dataset Size:** 310 entries, no missing values

## **Machine Learning Models Used**
- **Logistic Regression**
- **Support Vector Machine (SVM)** (Linear, Polynomial, RBF Kernels)
- **Decision Tree Classifier**
- **Random Forest Classifier**
- **Dimensionality Reduction Techniques:**
  - PCA (Principal Component Analysis)
  - LDA (Linear Discriminant Analysis)
  - PLS (Partial Least Squares)

## **Feature Selection & Importance**
- **Top features identified:**
  - **Degree Spondylolisthesis** & **Sacral Slope** appeared in all models, proving their critical role in distinguishing between Normal and Abnormal conditions.
  - Other important features include **Pelvic Tilt, Pelvic Incidence, and Thoracic Slope**.

## **Results & Findings**
| Model | Accuracy |
|--------|---------|
| **SVM (Linear Kernel)** | **87% (Best performer)** |
| Logistic Regression | High recall for abnormal cases |
| SVM (RBF Kernel) | Competitive results |
| Decision Tree & Random Forest | Struggled with class imbalance |

- **SVM (Linear Kernel) achieved the highest performance (87%)**.
- Logistic Regression showed good recall for **abnormal cases** but had lower precision.
- **Decision Tree and Random Forest** struggled with class imbalance issues.



## **Installation & Setup**
Clone the repository and install the dependencies:
```bash
git clone https://github.com/jadavbindupriya/Spinal_Condition_Analysis.git
cd Spinal_Condition_Analysis
pip install -r requirements.txt
```

## **Usage**
Run the notebook for analysis in **Google Colab**:
```python
# Open the project in Google Colab
https://colab.research.google.com/drive/1lv0D7FOM0msb3GAr0K3bjUfhcBavC7HW
```




