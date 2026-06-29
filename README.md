# Smart Outcome Predictor

This project uses ensemble learning methods to predict student outcomes on an EdTech platform.

## Tasks
1. **Classification** - Predict if a student will complete the course (completion_status)
2. **Regression** - Predict the final score of a student (final_score)

## Dataset
5200 student records with features like age, sessions, time spent, quiz scores, attendance etc.

## Steps Done
- Dropped student_id and course_start_date
- Encoded categorical columns using LabelEncoder
- Handled missing values with median imputation
- Scaled features using StandardScaler
- Split 80-20 for train-test

## Models Used
- **Bagging** - Bagging Classifier and Regressor (100 trees)
- **AdaBoost** - Classifier and Regressor
- **Gradient Boosting** - Classifier and Regressor
- **LightGBM** - Classifier and Regressor
- **XGBoost** - Classifier and Regressor
- **Voting** - Hard and Soft Voting Classifier
- **Stacking** - Stacking Classifier and Regressor

## Results
- Ensemble methods performed better than single decision tree
- XGBoost and LightGBM gave the best results among boosting methods
- Stacking also performed well by combining multiple models
- Most important features: quiz scores, time spent, attendance rate

## Files
- `PROJECT 5.ipynb` - Main notebook with code and analysis
- `theory_concepts.pdf` - Theory document
- `README.md` - This file
