# LW5_Comparative_Analysis

# Google Colab Link Here: https://colab.research.google.com/drive/1BsKmapHQ0sFxUycZq2Yhay3YGKHIaEo3?usp=sharing

# GUIDE QUESTIONS (FINAL REFLECTION)

# A. Model Performance

# 1. Which pre-trained model achieved the highest accuracy? Why?
- The MobileNetV2 model achieved the highest accuracy with 90.43%. This may be because MobileNetV2 was able to extract image features more effectively and generalize better on the crop species dataset compared to the other models.

# 2. Which model had the lowest performance? What could be the reason?
- The EfficientNetB0 model had the lowest performance with an accuracy of 5.50%. A possible reason is that the model may not have adapted well to the dataset configuration, insufficient training time, or ineffective feature extraction for the given crop images.

# 3. How did loss values compare across models?
- The MobileNetV2 model showed lower loss values, indicating better learning and prediction capability. In contrast, EfficientNetB0 and ResNet50 had higher loss values, suggesting weaker performance and poor model convergence.


# B. Evaluation Metrics

# 4. Why is accuracy not enough to evaluate a model?
-Accuracy alone is not enough because it only measures the percentage of correct predictions. Other metrics such as Precision, Recall, and F1-score provide deeper insights into false positives and false negatives, helping evaluate model reliability more effectively.

# 5. Which model had the best F1-score? What does it indicate?
-The MobileNetV2 model achieved the highest F1-score of 0.9034. This indicates a strong balance between precision and recall, meaning the model performed consistently well in identifying crop classes correctly.

# 6. How did Precision and Recall differ across models?
- The MobileNetV2 model had high precision (0.9064) and recall (0.9043), showing balanced performance. Meanwhile, EfficientNetB0 and ResNet50 had significantly lower precision and recall, indicating difficulties in correctly identifying crop classes.


# C. Confusion Matrix Analysis

# 7. Which classes were frequently misclassified?
- Classes such as ramie, ube, and saffron were more frequently misclassified in the MobileNetV2 model because they showed relatively lower recall and F1-scores compared to other classes. In weaker models, many classes were heavily misclassified due to poor prediction performance.

# 8. What patterns did you observe in the confusion matrix?
-The confusion matrix showed that MobileNetV2 had stronger diagonal values, meaning most predictions were correct. In contrast, EfficientNetB0 and ResNet50 displayed scattered misclassifications, indicating poor class recognition.

# D. ROC and AUC

# 9. Which model had the highest AUC score?
- The MobileNetV2 model achieved the highest AUC score of 0.9966, outperforming EfficientNetB0 (0.5071) and ResNet50 (0.5961).

# 10. What does AUC tell us about model performance?
- The AUC (Area Under the Curve) measures the model’s ability to distinguish between classes. A higher AUC score indicates better classification performance and stronger discrimination capability between categories.


# E. Explainability (Grad-CAM)

# 11. What did Grad-CAM reveal about model decision-making?
- Grad-CAM revealed which regions of the crop images influenced the model’s predictions. It helped visualize how the model focused on important plant features before making classification decisions.

# 12. Did the model focus on relevant image regions?
- Yes, the MobileNetV2 model focused more on relevant image regions, such as leaf and plant structures, which contributed to more accurate predictions. The weaker models showed less meaningful attention patterns.

# 13. Which model produced the most meaningful heatmaps?
- The MobileNetV2 model produced the most meaningful heatmaps because it highlighted relevant crop regions more clearly, making its predictions easier to interpret.

# F. Model Comparison & Improvement

# 14. Which model would you recommend for deployment? Why?
- The MobileNetV2 model is recommended for deployment because it achieved the highest accuracy, precision, recall, F1-score, and AUC score, making it the most reliable and efficient model for crop classification.

# 15. How can you further improve your best-performing model?
- The model can be further improved by applying data augmentation, hyperparameter tuning, increasing training data, fine-tuning deeper layers, and optimizing learning rates to improve generalization performance.


# G. Real-World Application

# 16. How can your model be applied in real-world scenarios?
- The model can be applied in agriculture to identify crop species automatically, assist farmers in crop monitoring, improve agricultural management, and support smart farming systems.

# 17. What are the risks of deploying an inaccurate model?
- An inaccurate model may lead to incorrect crop classification, poor agricultural decisions, reduced productivity, and financial losses due to wrong recommendations.

# 18. How can this system be integrated into a mobile/web app?
- The system can be integrated into a mobile or web application where users upload crop images, and the trained AI model predicts the crop species instantly. This can help farmers and agricultural experts access quick and accurate crop identification.
