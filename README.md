# ML_ImplimentedExample
## Topic 1 - Pre-Pruning and Post-Pruning 

Pre-pruning and post-pruning are techniques used in decision tree algorithms to prevent overfitting and improve generalization:

- Pre-pruning (Early Stopping): This involves halting the tree growth early, before it reaches its maximum size. Constraints like a maximum depth, minimum number of samples per leaf, or a minimum information gain threshold are applied during tree construction to stop splitting nodes. While it reduces overfitting, it risks underfitting by stopping the tree too early.

- Post-pruning (Prune After Full Growth): The tree is fully grown, and then unimportant branches are removed. This involves evaluating nodes and pruning them if their removal doesn't significantly decrease performance (e.g., based on cross-validation or statistical tests). Post-pruning balances complexity and performance better but is computationally more intensive.

## Topic 2 - Confusion Matrix, Recall, and Precision

**Confusion Matrix**:  
A confusion matrix is a performance measurement tool used in classification problems to evaluate how well a model predicts outcomes. It is a tabular representation of the actual vs. predicted outcomes. It has four key components:  
- **True Positives (TP)**: Correctly predicted positive cases.  
- **True Negatives (TN)**: Correctly predicted negative cases.  
- **False Positives (FP)**: Negative cases incorrectly predicted as positive (Type I error).  
- **False Negatives (FN)**: Positive cases incorrectly predicted as negative (Type II error).  

---

**Recall (Sensitivity or True Positive Rate)**:  
Recall measures the model's ability to identify all relevant positive cases. It is the proportion of actual positives that are correctly predicted.  

\[
\text{Recall} = \frac{\text{TP}}{\text{TP} + \text{FN}}
\]  
A high recall indicates the model successfully detects most positive cases but may misclassify some negatives as positives.

---

**Precision (Positive Predictive Value)**:  
Precision evaluates the accuracy of positive predictions. It is the proportion of predicted positives that are correctly classified.  

\[
\text{Precision} = \frac{\text{TP}}{\text{TP} + \text{FP}}
\]  
High precision means that most predicted positives are true positives, minimizing false alarms.

---

Both metrics are critical for understanding model performance, particularly in imbalanced datasets. For example, in spam email detection, recall ensures most spam emails are caught, while precision ensures non-spam emails aren't flagged incorrectly.
