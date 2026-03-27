SVM Kernel Comparison on Heart Disease Dataset
 Project Overview

This project explores how different Support Vector Machine (SVM) kernel functions affect classification performance on a heart disease dataset. The main objective is to compare Linear, Polynomial, and Radial Basis Function (RBF) kernels and understand their impact on model accuracy and decision boundaries.

 Objectives
Implement SVM models with different kernel functions
Analyse how kernel choice affects classification performance
Visualise decision boundaries using PCA
Evaluate models using multiple performance metrics
 Dataset

The dataset used is a Heart Disease Dataset, commonly used for binary classification problems.

Features include:
Age
Sex
Chest pain type
Resting blood pressure
Cholesterol level
Fasting blood sugar
Maximum heart rate
Target:
1 → Presence of heart disease
0 → Absence of heart disease

 Technologies Used
Python 
NumPy
Pandas
Matplotlib
Seaborn
Scikit-learn
 Data Preprocessing
Dataset split into training (70%) and testing (30%)
Feature scaling using StandardScaler
Data transformed using Principal Component Analysis (PCA) for visualization

 Exploratory Data Analysis (EDA)
Correlation matrix used to identify relationships between features
Target variable distribution checked for class balance
Insights used to improve model performance

 Dimensionality Reduction
PCA applied to reduce features to 2 components
Helps in:
Visualising decision boundaries
Reducing computational complexity
Minimising noise

SVM Kernel Functions
🔹 Linear Kernel
Best for linearly separable data
Fast and computationally efficient
🔹 Polynomial Kernel
Captures feature interactions
Performance depends on polynomial degree
🔹 RBF Kernel
Handles complex non-linear data
Uses Gaussian similarity function
Generally provides highest accuracy

 Model Training

Three SVM models were trained using:

Linear Kernel
Polynomial Kernel
RBF Kernel

Each model learns an optimal decision boundary using support vectors.

 Model Evaluation

Models are evaluated using:

Accuracy
Confusion Matrix
Precision
Recall
F1-Score

These metrics provide a complete understanding of performance.

 Results
Linear Kernel → Works well for simple patterns
Polynomial Kernel → Better for moderate complexity
RBF Kernel → Best performance for complex data

 RBF kernel achieved the highest accuracy in most cases.

 Decision Boundary Visualization
PCA-reduced data used for 2D plotting
Linear → Straight boundary
Polynomial → Curved boundary
RBF → Highly flexible boundary

 Key Insights
Kernel selection significantly impacts SVM performance
RBF kernel is most effective for non-linear datasets
PCA improves visualization and efficiency
Feature scaling is critical for SVM models

 Conclusion

This project demonstrates that SVM is a powerful classification algorithm, especially when combined with the right kernel. Among all kernels tested, the RBF kernel provides the best performance for complex datasets like heart disease prediction.

 How to Run
# Clone the repository
git clone https://github.com/your-username/svm-kernel-comparison.git

# Navigate to project folder
cd svm-kernel-comparison

# Install dependencies
pip install -r requirements.txt

# Run the script
python main.py
 Project Structure
├── data/
├── notebooks/
├── src/
├── images/
├── requirements.txt
└── README.md

