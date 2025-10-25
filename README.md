# 🔢 Normalization

---

## 🧰 Libraries Used
- numpy  
- pandas  
- matplotlib  
- seaborn  
- sklearn (MinMaxScaler)

---

## 📊 Dataset
Dataset is in the repo.  
It has 3 class labels.

---

## 📖 Steps

### 1️⃣ Data Exploration
- Took data  
- Saw distribution plot of one feature → <img width="576" height="432" alt="norm1" src="https://github.com/user-attachments/assets/cf6b2f7b-a28a-4a44-a529-916120b80f55" />

- Saw distribution of 2nd feature “Malic Acid” → <img width="567" height="432" alt="norm2" src="https://github.com/user-attachments/assets/e27ced07-5764-4352-abec-a184367e3498" />
  
- 3 class labels are present  
- Plotted them on scatter plot → *<img width="567" height="434" alt="norm3" src="https://github.com/user-attachments/assets/c87ece6d-1ecb-4438-88f2-cdec2459799a" />


---

### 2️⃣ Train-Test Split and Normalization
- Performed train-test split  
- Imported `MinMaxScaler` from sklearn  
- Fit and transformed data using it  

After transformation:
- Min = 0  
- Max = 1  
- Mean and Std also decreased  

---

### 3️⃣ Visualization and Comparison
- Plotted scatter plot before and after scaling → *<img width="968" height="451" alt="norm4" src="https://github.com/user-attachments/assets/92d90c62-7d03-4f48-ade7-3ea398ed02e1" />
*  
  - Data is same, just scale changed  

- Plotted KDE plot before and after → *<img width="1001" height="470" alt="norm5" src="https://github.com/user-attachments/assets/394f85c6-c84f-4494-b487-72a24bff7184" />
*  
  - Range increased and width more spread  

- Plotted distribution plot before and after of a feature → *<img width="1010" height="470" alt="norm6" src="https://github.com/user-attachments/assets/847be32f-69f3-4723-a6dd-b859273fe0d1" />
*  
  - Shape remained same across  

---

## ✅ Summary
- Normalization scaled all features between 0 and 1  
- Distribution and shape of data stayed same  
- Helps models that depend on distance (like KNN or SVM) perform better
