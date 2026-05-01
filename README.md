# -Laboratory-Work-4-Activity-Improving-CNN-Performance-Using-Regularization

https://colab.research.google.com/drive/1bQCcPy9UI9EoBkwzEgf-M6OM-hzgcuBQ?usp=sharing

GUIDE QUESTIONS (Student Explanation & Reflection)
A. Model Evaluation Analysis

1. What were the weakest-performing classes based on the confusion matrix?
Ans:. Weakest-Performing Classes
Classes with low diagonal values and high off-diagonal values in the confusion matrix are the weakest. Visually similar classes (e.g., cat, dog, deer) are most commonly misclassified due to shared features.


2. How did Precision, Recall, and F1-score vary across classes?
Ans:Precision, Recall, and F1-score Variation
Visually distinct classes (e.g., airplane, ship) score high across all three metrics, while visually ambiguous classes (e.g., cat, dog) score low. F1-score reflects the combined weakness of both precision and recall.


3. What does a low recall indicate in your model?
Ans:Low Recall
Low recall means the model misses many actual instances of a class, producing high false negatives. It usually happens when a class is visually similar to others or underrepresented in training data.

4. How does AUC score reflect model performance compared to accuracy?
Ans:AUC vs. Accuracy
Accuracy can be misleading with imbalanced data since it favors the majority class. AUC is more reliable as it measures the model's ability to distinguish between classes across all thresholds a high accuracy but low AUC signals the model is biased toward dominant classes.
