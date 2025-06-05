# Support Vector Machines (SVM) - Binary Classification

##  Objective
Use Support Vector Machines (SVMs) for binary classification with both **linear** and **non-linear (RBF)** kernels. This project focuses on understanding how SVM works, how decision boundaries change based on kernels, and how hyperparameter tuning improves model performance.

---

##  Tools & Libraries Used

- Python
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- PCA (for 2D visualization)

---

##  Dataset

- **Name:** breast-cancer.csv
- **Source:** Uploaded by user
- **Target Variable:** `diagnosis`  
  - Malignant = 1  
  - Benign = 0  
- **Features:** 30 numerical features extracted from digitized images of breast mass.

---

##  Tasks Performed

1. **Data Preprocessing**
   - Dropped unnecessary columns (e.g., `id`)
   - Encoded diagnosis (`M` → 1, `B` → 0)
   - Standardized features using `StandardScaler`

2. **Dimensionality Reduction**
   - Used **PCA** to reduce features to 2D for visualization

3. **Model Training**
   - Trained SVM with **Linear kernel**
   - Trained SVM with **RBF kernel**

4. **Visualization**
   - Plotted decision boundaries in 2D PCA space for both linear and RBF models

5. **Hyperparameter Tuning**
   - Used `GridSearchCV` to find the best `C` and `gamma` for RBF kernel

6. **Model Evaluation**
   - Classification Report (Precision, Recall, F1-score)
   - Cross-validation to check model stability and accuracy

---

##  Results

- RBF Kernel SVM performed better than Linear Kernel due to non-linearly separable data
- Best hyperparameters found using grid search
- Mean cross-validation accuracy: ~98-99% (depending on seed and params)

---


## 📘 What I Learned

- **Margin Maximization:** SVM works by finding the optimal hyperplane that maximizes the margin between classes.
- **Kernel Trick:** With RBF kernel, SVM can handle non-linear data by projecting it into higher-dimensional space.
- **Hyperparameter Tuning:** How `C` (regularization) and `gamma` (kernel influence) impact the decision boundary and overfitting.
- **Cross-validation:** Essential for validating model generalization and avoiding overfitting.
- **Visualization:** PCA can simplify and visualize high-dimensional classification problems.

---

## 🧠 Summary

This project gave hands-on experience with one of the most powerful classification algorithms—SVM. By visualizing, tuning, and evaluating the model, the key concepts of margin, kernel tricks, and generalization were solidified.

