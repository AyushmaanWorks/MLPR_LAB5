# MLPR_LAB5
This repository implements the K-Nearest Neighbors algorithm and explores how the choice of k affects model performance. It analyzes the bias–variance tradeoff, showing how small k can lead to overfitting while large k may cause underfitting. 


## Aim

- Implement the KNN algorithm using standard tools  
- Examine how varying **k** affects predictions  
- Develop an intuitive understanding of overfitting and underfitting  
- Use visualizations to interpret model behavior  

---

## Methodology

1. **Data Preparation**
   - Load and preprocess the dataset  
   - Apply feature scaling when required  

2. **Model Training**
   - Train KNN models with multiple values of k  
   - Measure classification accuracy  

3. **Performance Analysis**
   - Compare training and validation accuracy  
   - Evaluate prediction stability  
   - Study the bias–variance relationship  

4. **Visualization**
   - Generate decision boundary plots  
   - Compare smoothness across different k values  
   - Plot accuracy as a function of k  

---

## Key Observations

- **Small k (for example, k = 1)**
  - Highly detailed decision boundary  
  - Low bias  
  - High variance  
  - Susceptible to overfitting  

- **Large k**
  - More generalized decision boundary  
  - Reduced variance  
  - Increased bias  
  - Risk of underfitting  

Best performance is typically achieved at an intermediate value of k.

---

## Visualizations

### Decision Boundary (Small k)

![Decision Boundary Small K](images/decision_boundary_small_k.png)

### Decision Boundary (Large k)

![Decision Boundary Large K](images/decision_boundary_large_k.png)

### Accuracy vs k

![Accuracy Plot](images/accuracy_vs_k.png)

*(Ensure these images are saved in an `images/` folder within the repository.)*

---

## Conclusion

The experiment highlights how the parameter k determines the flexibility and generalization ability of a KNN model. Smaller values make the model sensitive to noise, while larger values simplify the decision boundary and may overlook important patterns. Choosing an appropriate k is crucial to maintaining a proper balance between bias and variance.

---

## Tools and Libraries

- Python  
- NumPy  
- Matplotlib  
- scikit-learn  

---

## Running the Project

1. Clone the repository  
2. Install the necessary dependencies  
3. Open the notebook file  
4. Execute all cells  

---

## Author

Your Name  
Machine Learning and Pattern Recognition  
Spring 2026
