# Dataset Description

This document describes the schema of the `student_habits_performance.csv` dataset used in the Student Exam Score Prediction project.

## Columns
| Column Name                   | Type   | Description                                      |
|-------------------------------|--------|--------------------------------------------------|
| student_id                    | int    | Unique identifier for each student (dropped)      |
| age                           | int    | Age of the student (e.g., 15-25)                 |
| study_hours_per_day           | float  | Hours spent studying per day                     |
| social_media_hours            | float  | Hours spent on social media per day              |
| netflix_hours                 | float  | Hours spent watching Netflix per day             |
| attendance_percentage          | float  | Percentage of classes attended                   |
| sleep_hours                   | float  | Hours of sleep per night                         |
| exercise_frequency            | float  | Days per week of exercise                        |
| mental_health_rating          | int    | Self-reported mental health rating (1-10)        |
| diet_quality                  | string | Diet quality (Poor, Fair, Good)                  |
| parental_education_level      | string | Parent's education (High School, Bachelor, Master)|
| internet_quality              | string | Internet quality (Poor, Average, Good)           |
| gender                        | string | Gender (Male, Female)                            |
| part_time_job                 | string | Has part-time job (Yes, No)                      |
| extracurricular_participation  | string | Participates in extracurriculars (Yes, No)        |
| exam_score                    | float  | Exam score (0-100, target variable)              |

## Notes
- The dataset is synthetic and does not contain real student data.
- Missing values may exist and are handled in the preprocessing pipeline.
- The `student_id` column is dropped during modeling as it is not a predictive feature.