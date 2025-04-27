# Student Exam Score Prediction

## Overview
This project aims to predict students' exam scores (`exam_score`) based on their study habits and lifestyle factors, such as study hours, social media usage, sleep hours, and more. The goal is to identify key factors influencing academic performance and provide insights for students and educators.

## Dataset
- **Source**: Synthetic dataset (`student_habits_performance.csv`) simulating student habits and performance.
- **Features**: 12 features including `age`, `study_hours_per_day`, `social_media_hours`, `diet_quality`, `gender`, etc.
- **Target**: `exam_score` (on a 0-100 scale).
- **Size**: [Specify size, e.g., 1000 rows; update based on your data].

For detailed feature descriptions, see [data_description.md](data_description.md).

## Tools and Libraries
- Python 3.8+
- Libraries: `pandas`, `scikit-learn`, `ydata-profiling`, `seaborn`, `matplotlib`, `numpy`

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/student-performance-prediction.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Ensure the dataset (`student_habits_performance.csv`) is in the `data/` folder.

## Usage
1. Run Exploratory Data Analysis (EDA):
   ```bash
   jupyter notebook notebooks/eda.ipynb
   ```
2. Train and evaluate the model:
   ```bash
   python src/main.py
   ```

## Results
- **Model**: LassoLarsCV with RandomizedSearchCV
- **R² (Test)**: 0.8986
- **RMSE (Test)**: 5.10 (on a 0-100 scale)
- **Key Findings**: Study hours and attendance percentage are strong predictors of exam scores.

## Project Structure
```
student-performance-prediction/
├── data/                          # Dataset
├── figures/                       # Visualizations (e.g., correlation heatmap)
├── src/                           # Source code
│   ├── main.py                    # Main script to run the pipeline
│   ├── data_preprocessing.py      # Preprocessing pipeline
│   ├── model_training.py          # Model training and hyperparameter tuning
│   ├── evaluation.py              # Model evaluation and visualization
├── notebooks/                     # Jupyter notebooks
│   ├── eda.ipynb                  # Exploratory Data Analysis
├── README.md                      # Project overview
├── requirements.txt               # Dependencies
├── data_description.md            # Dataset schema
├── .gitignore                     # Git ignore file
├── LICENSE                        # License
```

## Visualizations
![Correlation Heatmap](figures/correlation_heatmap.png)
![Exam Score by Gender](figures/exam_score_boxplot.png)

## Author
- [Your Name] (https://linkedin.com/in/your-profile)
- GitHub: [your-username](https://github.com/your-username)

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.