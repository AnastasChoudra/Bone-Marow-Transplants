# Bone-Marrow Transplant (Children) – Survival Classification

Dataset  
[UCI “Bone Marrow Transplant Children”](https://archive.ics.uci.edu/dataset/565/bone+marrow+transplant+children)  
37 clinical variables, 187 patients, target: survival_status (0 = alive, 1 = dead).

Project  
End-to-end scikit-learn **Pipeline** that  
- imputes & one-hot-encodes categorical vars (≤ 7 unique values)  
- imputes & standard-scales numeric vars (> 7 unique values)  
- reduces dimensionality with PCA  
- classifies with Logistic Regression + hyper-parameter tuning (C, PCA components)

Results  
Best test accuracy: **76.3 %**  
Chosen PCA components: 30  
Logistic Regression: C = 100  
(5-fold GridSearchCV, random-state = 1, 80/20 train-test split)

