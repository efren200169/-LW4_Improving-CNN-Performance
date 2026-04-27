# -LW4_Improving-CNN-Performance 
https://colab.research.google.com/drive/1L3l57K0lfNquROtEza58N-67f9xODin7?usp=drive_link
## GUIDE QUESTIONS (Student Explanation & Reflection)

A. Model Evaluation Analysis
1. What were the weakest-performing classes based on the confusion matrix?
- From the confusion matrix, the weakest classes were the ones that the model kept mixing up with others. Usually, these are classes that look similar or don’t have enough training data, so the model struggles to tell them apart.
2. How did Precision, Recall, and F1-score vary across classes?
- These scores weren’t the same for every class. Some classes had good precision but lower recall, meaning the model was careful but missed some actual cases. Others had higher recall but lower precision, meaning it caught more cases but also made more mistakes. The F1-score helped balance both.
3. What does a low recall indicate in your model?
- Low recall means the model is missing a lot of actual examples of that class. In simple terms, it’s not good at detecting that class when it’s really there.
4. How does AUC score reflect model performance compared to accuracy?
- Accuracy just tells how many predictions were correct overall, but AUC shows how well the model separates classes across different thresholds. So even if accuracy isn’t super high, a good AUC means the model still has strong classification ability.

B. Model Improvement
6. How did data augmentation affect validation accuracy?
- Data augmentation helped improve validation accuracy because it gave the model more varied examples to learn from. This made it better at handling new, unseen data.
7. Why is Batch Normalization important in CNNs?
- Batch Normalization helped make training faster and more stable. It keeps the values in each layer balanced, which makes learning more efficient.
8. What role did Dropout play in improving your model?
- Dropout helped prevent overfitting by randomly turning off some neurons during training. This forced the model to learn more general patterns instead of memorizing.
9. How did Early Stopping prevent overfitting?
- Early stopping prevented overfitting by stopping training once the validation performance stopped improving. This avoids the model learning noise from the training data.
    
C. Performance Comparison
11. What improvements were observed after modifying the model?
- After improving the model, the validation accuracy increased and the loss decreased. The model also performed more consistently on new data.
12. Which enhancement contributed the most to performance improvement? Why?
- Data augmentation and Dropout probably helped the most because they improved how well the model generalizes, not just memorizes.
13. Did the gap between training and validation accuracy decrease? Explain.
- The gap between training and validation accuracy became smaller, which is a good sign. It means the model is no longer overfitting as much.

D. Explainability (Grad-CAM Integration)
14. How did Grad-CAM help in understanding model predictions?
- Grad-CAM made it easier to see what parts of the image the model was focusing on when making predictions.
15. Did the improved model focus on more relevant regions? Provide evidence.
- Yes, the improved model focused more on the important parts of the image instead of random background areas, which shows it learned better features.
16. Why is explainability important in real-world AI applications?
- Explainability is important because it helps people trust the model. It also helps us understand mistakes and make improvements, especially in real-world situations.
