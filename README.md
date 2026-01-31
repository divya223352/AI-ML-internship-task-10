# AI-ML-internship-task-10
1. Why Feature Scaling is Mandatory
In your dataset, each pixel is a feature. KNN is highly sensitive to the magnitude of data.
If one feature (Pixel A) ranges from 0 to 1 and another (Pixel B) ranges from 0 to 255, the distance calculation will be dominated by Pixel B.
StandardScaler transforms the data so that all features have a mean of 0 and a standard deviation of 1, giving every pixel an equal "vote" in the distance calculation.
2. The Role of "K" (Hyperparameter Tuning)
Choosing the right K is a balancing act:
Small K (e.g., K=1): The model is too sensitive to noise and outliers (Overfitting).
Large K: The model becomes too "blurred" and might pick the most common class in the whole dataset rather than the local neighbors (Underfitting).
3. Deliverables Explained
Confusion Matrix: A table used to describe the performance of a classification model. It shows exactly which digits are being confused (e.g., if the model often mistakes "8" for "1").
Accuracy vs. K Plot: This graph helps you find the "Elbow" or the peak where accuracy is highest, helping you choose the optimal K for your specific data.
