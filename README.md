Breast Cancer Classification using KNN

📝 Objective:

Classify breast tumors as malignant or benign using K-Nearest Neighbors (KNN) algorithm.

⸻

🔑 Features Used:
	•	radius_mean
	•	texture_mean
	•	perimeter_mean
	•	area_mean
	•	smoothness_mean
	•	compactness_mean
	•	concavity_mean
	•	concave_points_mean
	•	… (and other related features from the dataset)

Target column: diagnosis
	•	M = Malignant
	•	B = Benign

⸻

🧪 Steps Followed:
	1.	Import necessary libraries (sklearn, pandas, numpy, etc.)
	2.	Load and inspect the dataset
	3.	Drop irrelevant columns like id
	4.	Convert labels: diagnosis → 0 (Benign), 1 (Malignant)
	5.	Split data into training and testing sets (80/20)
	6.	Normalize features using StandardScaler
	7.	Train KNN model using KNeighborsClassifier
	8.	Evaluate using:
	•	Accuracy score
	•	Classification report
	•	Confusion matrix
	9.	Plot error rate vs K to find optimal number of neighbors

⸻

✅ Highlights:
	•	Simple and effective KNN model
	•	Well-preprocessed data
	•	Easily customizable for tuning K value
	•	Good baseline for medical classification tasks

⸻

Let me know if you want to include the error plot image or accuracy score result in this too!
