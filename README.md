# Random Forest Algorithm Project

## Overview
This project implements a Random Forest algorithm to predict whether students will pass or fail based on their exam scores and attendance. The dataset used is `school_data.csv`, which contains three columns: `Exam Score`, `Attendance`, and `Pass/Fail`.

## Dataset
The dataset contains the following features:
- **Exam Score**: The score obtained by the student in an exam.
- **Attendance**: The total attendance of the student.
- **Pass/Fail**: The target variable indicating whether the student passed (1) or failed (0).

### Sample Data
| Exam Score | Attendance | Pass/Fail |
|------------|------------|-----------|
| 81         | 169        | 1         |
| 44         | 95         | 0         |
| 90         | 104       | 0         |

## Visualizations
A scatter plot is created to visualize the relationship between `Exam Score` and `Attendance`, colored by the `Pass/Fail` status.

```python
import seaborn as sns
import matplotlib.pyplot as plt

sns.scatterplot(x="Exam Score", y="Attendance", hue="Pass/Fail", data=dataset)
plt.show()
