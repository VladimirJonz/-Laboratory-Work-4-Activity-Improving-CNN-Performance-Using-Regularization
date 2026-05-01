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

B. Model Improvement

5. How did data augmentation affect validation accuracy?
Ans: Data Augmentation and Validation Accuracy
Data augmentation (flipping, rotating, cropping, etc.) exposes the model to more varied training samples, reducing overfitting and improving generalization. This leads to better validation accuracy because the model learns features that are position- and orientation-invariant rather than memorizing specific training images.


6. Why is Batch Normalization important in CNNs?
Ans: Importance of Batch Normalization in CNNs
Batch Normalization normalizes layer inputs during training, keeping activations in a stable range. This speeds up training, reduces sensitivity to weight initialization, and acts as a mild regularizer — allowing higher learning rates and leading to faster convergence and better overall performance.
7. What role did Dropout play in improving your model?
Ans: Role of Dropout in Model Improvement
Dropout randomly deactivates a fraction of neurons during training, forcing the network to learn redundant and distributed representations. This prevents co-adaptation of neurons, reduces overfitting, and improves the model's ability to generalize to unseen data.

8. How did Early Stopping prevent overfitting?
Ans:How Early Stopping Prevented Overfitting
Early stopping monitors validation loss during training and halts the process once it stops improving. This prevents the model from continuing to train past the point where it starts memorizing training data, effectively preserving the best-performing model weights before overfitting occurs.

B. Model Improvement
