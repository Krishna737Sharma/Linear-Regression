# Linear Regression  

## Objective  
To predict the final year grades (G3) of students using linear regression. The dataset contains binary, integer, and continuous features, requiring preprocessing, one-hot encoding, and feature scaling. The linear regression model is implemented from scratch with gradient descent and learning rate scheduling.

---

## Tasks  

### **Task 1: Load Dataset**  
- Loaded the **Student Performance** dataset from [UCI Repository](https://archive.ics.uci.edu/dataset/320/student+performance).  

---

### **Task 2: Data Preprocessing**  
1. **Check for Missing and Duplicate Values**:  
   - Removed duplicates and handled missing values appropriately.

2. **Feature Selection**:  
   - Excluded columns `G1` and `G2` as they are not features.

3. **One-Hot Encoding**:  
   - Performed one-hot encoding for categorical features.
   - Represented a feature with *k* distinct values using (*k-1*) binary features.
   - **Number of features after encoding**: `<value>`.

4. **Feature Scaling**:  
   - Scaled all features to ensure their values lie within the same range.

---

### **Task 3: Splitting the Dataset**  
- Split the dataset into:
  - **70% Training Set**
  - **15% Validation Set**
  - **15% Test Set**  

---

### **Task 4: Linear Regression Implementation**  
1. **Implemented Linear Regression from Scratch**:  
   - Used **gradient descent** to minimize the **mean squared error (MSE)** loss function.

2. **Learning Rate Scheduling**:  
   - Initial learning rate: `0.1`.  
   - Reduced by a factor of `0.1` if validation loss does not improve for `10` consecutive steps.  
   - Stopped training when:
     - Learning rate ≤ `10^-5`.  
     - Validation loss did not improve further.  

---

### **Task 5: Evaluation and Visualization**  
1. **Loss Progression**:  
   - Plotted training and validation losses against the number of iterations.

2. **Test Set MSE**:  
   - Calculated and reported the mean squared error on the test set.

3. **Scatter Plot**:  
   - Plotted predicted grades vs. true grades on the test set.  

---

## Results  

### **Test Set Performance**  
- **Mean Squared Error (MSE)**: `<value>`  

### **Visualizations**  
1. **Loss Progression**:  
   - Training Loss vs. Iterations.  
   - Validation Loss vs. Iterations.  

2. **Scatter Plot**:  
   - Predicted Grades vs. True Grades.  

---

## How to Run  

1. Install required libraries:  
   ```bash
   pip install numpy pandas matplotlib scikit-learn
