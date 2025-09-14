# Diabetes Data Visualization

## Project Description
This project visualizes a diabetes dataset using Python, Matplotlib, and Seaborn.  
The goal is to explore relationships between patient features (like Age, Glucose, BMI) and diabetes outcomes.  
It includes multiple types of visualizations to gain insights into the dataset and highlight important patterns.

---

## Dataset
The dataset contains patient information for diabetes diagnosis with the following columns:
Dataset used from kaggle CSV file.
| Column | Description |
|--------|-------------|
| Pregnancies | Number of times pregnant |
| Glucose | Plasma glucose concentration |
| BloodPressure | Diastolic blood pressure (mm Hg) |
| SkinThickness | Triceps skinfold thickness (mm) |
| Insulin | 2-Hour serum insulin (mu U/ml) |
| BMI | Body Mass Index (weight in kg/(height in m)^2) |
| DiabetesPedigreeFunction | Function to indicate diabetes likelihood based on family history |
| Age | Age of the patient |
| Outcome | Diabetes outcome (0 = No, 1 = Yes) |

## Visualizations

### 1. Distribution of Key Patient Features(Histogram)
This set of graphs shows the distribution of each numeric feature in the dataset.
- Peaks indicate common values for each feature (e.g., Glucose, BMI, Age).
- Helps identify skewness, spread, and patterns in the data.
- Provides a quick overview of how patients’ health metrics vary.

<img width="1031" height="687" alt="image" src="https://github.com/user-attachments/assets/65ec57e3-60f4-4452-8434-8158cbcdf9bb" />

### 2. Glucose Levels by Diabetes Outcome(Violin Plot)
This graph shows the distribution of Glucose levels for each diabetes outcome (0 = Non-Diabetic, 1 = Diabetic).
- Distribution Shape: The width at each glucose level indicates how many patients have that value. Wider sections mean more common values.
- Median and Quartiles: Central tendency and spread of glucose levels are visible.
- Comparison Between Outcomes: Non-Diabetic patients mostly have lower glucose values. Diabetic patients tend to have higher glucose values, indicating a strong association between high glucose and diabetes.
- Density Peaks: Highlights clusters or patterns in glucose levels for each group.

<img width="855" height="614" alt="image" src="https://github.com/user-attachments/assets/119bef93-a0e7-4239-9d24-0bd783493402" />

### 3. BMI Levels by Diabetes Outcome(Swarm Plot)
This graph shows the distribution of BMI (Body Mass Index) values for each diabetes outcome (0 = Non-Diabetic, 1 = Diabetic).
- Individual Data Points: Each point represents a patient’s BMI, showing how values are spread within each group.
- Comparison Between Outcomes: Non-Diabetic patients mostly have lower to moderate BMI values. Diabetic patients tend to have higher BMI values, suggesting a correlation between higher BMI and diabetes risk.
- Spread and Clustering: You can see clusters and outliers clearly, making it easier to identify overlapping BMI ranges between diabetic and non-diabetic patients.

<img width="830" height="617" alt="image" src="https://github.com/user-attachments/assets/03ffb0df-b371-4a1b-b4c1-db0eb0582309" />

### 4. Age Distribution of Patients(Histogram + KDE)
This graph shows how patients are distributed across different ages in the dataset.
- Distribution Shape: The width of the bars indicates the number of patients in each age range. Peaks represent age ranges with more patients.
- Spread: It shows how ages vary across the dataset — whether most patients are young, middle-aged, or older.
- Density Curve: The smooth curve on top of the bars highlights the overall trend in age distribution, making it easier to see common age ranges.

<img width="1007" height="607" alt="image" src="https://github.com/user-attachments/assets/712ffe58-cb0a-4431-8cdd-54bbe0b11f16" />

### 5. Feature Comparison by Diabetes Outcome(Box Plot)
This set of graphs shows how different numeric features (Pregnancies, Glucose, BloodPressure, SkinThickness, Insulin, BMI, DiabetesPedigreeFunction, Age) vary between non-diabetic (Outcome = 0) and diabetic (Outcome = 1) patients.
- Central Tendency and Spread: The boxplots display the median, quartiles, and outliers for each feature, helping to understand the distribution within each group.
- Comparison Between Outcomes:

Glucose and BMI: Tend to be higher for diabetic patients, highlighting a strong association with diabetes.
Age: Shows differences in age distribution between diabetic and non-diabetic patients.
Other Features: Some features like BloodPressure, Insulin, and SkinThickness may show overlapping ranges but still reveal subtle differences.

- Outliers: Boxplots make it easy to identify extreme values that might influence analysis or model predictions.

<img width="1123" height="730" alt="image" src="https://github.com/user-attachments/assets/3f9b83d8-d5fa-4901-bf72-9d7ef44b8016" />

### 6. Relationship Between Glucose and BMI by Diabetes Outcome(Scatter Plot)
This graph shows the relationship between Glucose levels and BMI for patients, colored by their diabetes outcome (0 = Non-Diabetic, 1 = Diabetic).
- Feature Interaction: Each point represents a patient, plotting their Glucose and BMI values simultaneously.
- Outcome Comparison: Diabetic patients (Outcome = 1) tend to cluster in regions with higher Glucose and higher BMI. Non-diabetic patients (Outcome = 0) are mostly concentrated at lower Glucose and BMI values.
- Patterns and Trends: Helps visually identify correlations between Glucose and BMI in relation to diabetes.
- Outliers: Individual points outside the main clusters are easily visible, indicating extreme cases.

<img width="891" height="550" alt="image" src="https://github.com/user-attachments/assets/85abd61c-d9a1-404e-ad6f-b39333231e6a" />

### 7. Relationships Between Key Features and Diabetes Outcome(Pair Plot)
This graph shows the pairwise relationships between important features — Glucose, BMI, Age, and Insulin — with points colored by diabetes outcome (0 = Non-Diabetic, 1 = Diabetic).
- Feature Interactions: Each subplot compares two features, helping identify correlations, trends, and patterns.
- Outcome Comparison: Diabetic patients (Outcome = 1) tend to cluster at higher Glucose and BMI values. Non-diabetic patients (Outcome = 0) are mostly at lower values across these features.
- Distribution Insight: The diagonal subplots show the distribution of individual features for each outcome.

<img width="681" height="647" alt="image" src="https://github.com/user-attachments/assets/66f9b87f-5c6a-4843-bd29-4c93ec0ce0f7" />

### 8. Diabetes Outcome Across Number of Pregnancies(Heatmap)
This graph shows how the number of pregnancies relates to diabetes outcome (0 = Non-Diabetic, 1 = Diabetic) using a heatmap.
- Counts of Patients: Each cell shows the number of patients for a specific combination of pregnancies and outcome.
- Pattern Recognition: Helps identify whether higher number of pregnancies is associated with higher diabetes incidence. Non-diabetic patients (Outcome = 0) are concentrated in lower or moderate pregnancy counts. Diabetic patients (Outcome = 1) appear more in certain pregnancy ranges, indicating potential trends.

<img width="655" height="510" alt="image" src="https://github.com/user-attachments/assets/871d5fda-97cc-4587-9c21-9b11bf5fdde3" />

### 9. Diabetes Count by Age(Bar Graph)
This graph shows the number of diabetic patients at each age.
- Peaks indicate age groups with higher diabetes incidence.
- Helps quickly identify which ages are most affected.

<img width="1157" height="606" alt="image" src="https://github.com/user-attachments/assets/01796010-f47b-4e6d-9e7a-453c0d550db0" />

### 10. Proportion of Diabetic vs Non-Diabetic Patients(Donut)
This graph shows the percentage of patients with and without diabetes.
- Quickly visualizes the overall distribution of diabetes outcomes in the dataset.
- Highlights the proportion of high-risk patients relative to the total population.
  
<img width="597" height="608" alt="image" src="https://github.com/user-attachments/assets/4c3f423b-afd3-4310-bc10-d915ec3f3aab" />
