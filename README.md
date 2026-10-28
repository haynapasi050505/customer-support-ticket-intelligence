# Customer Support Ticket Intelligence

## Project Overview
This project analyses customer support tickets to identify issue patterns, resolution delays, escalation trends, and customer satisfaction. I also explored machine learning models to predict ticket priority.

## Business Objectives
- Analyse ticket volume by issue type, product, channel, and customer type.
- Identify issue types associated with longer resolution times.
- Understand patterns in escalation, reopened tickets, and customer satisfaction.
- Experiment with machine learning for ticket priority prediction.

## Tools Used
- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Google Colab
- GitHub

## Project Workflow
1. Loaded and inspected the dataset.
2. Checked missing values and duplicate records.
3. Cleaned the data and handled missing numeric values.
4. Performed exploratory data analysis and created visualisations.
5. Analysed ticket priority, resolution time, escalation, and customer satisfaction.
6. Trained and evaluated Random Forest and Decision Tree classification models.

## Key Findings
- Analysed 10,000 cleaned support ticket records.
- Bug and Login issues together represented approximately 34% of tickets.
- Integration issues had the longest average resolution time at 19.92 hours.
- Integration issues had the lowest average customer satisfaction at 3.55/5.
- Integration issues had the highest High-priority ticket share at 7.87%.
- Escalated tickets had a higher average resolution time than non-escalated tickets.

## Machine Learning Results
The dataset contained approximately 75.27% Low-priority tickets, 20.70% Medium-priority tickets, and 4.03% High-priority tickets.

The Random Forest model achieved approximately 75% accuracy on the test set but failed to identify High-priority tickets. A Decision Tree model achieved approximately 46% recall for High-priority tickets on a validation set, with approximately 14% precision.

These results highlight the challenge of predicting the minority class. The current models require further improvement and validation before any real-world use.

## Business Recommendations
- Investigate the reasons behind long resolution times for Integration issues.
- Review recurring Bug and Login issues.
- Examine escalation workflows and factors associated with delays.
- Monitor satisfaction and ticket reopening patterns.
- Improve High-priority ticket detection while controlling false alerts.

## Limitations
- Findings show associations and do not establish causation.
- The dataset has an imbalanced target variable.
- The models are experimental and are not ready for production use.

## Future Improvements
- Explore additional features available when a ticket is created.
- Test alternative approaches to class imbalance.
- Improve model performance using class-specific evaluation metrics.
- Validate results on additional data.

## Files
- `Customer_Support_Ticket_Intelligence.ipynb` — analysis, visualisations, and machine learning experiments.


