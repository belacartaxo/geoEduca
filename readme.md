# GeoEduca: Analyzing and Predicting PROUNI Cutoff Scores with Geographic Context

## Overview
The Programa Universidade para Todos (**PROUNI**) is a Brazilian government initiative that provides scholarships for students to access private higher education institutions. Scholarships are granted based on cutoff scores determined by the National High School Exam (**ENEM**) and are categorized as full (100%) or partial (50%) based on socioeconomic criteria. These scholarships are vital for increasing accessibility to higher education across Brazil.

This project, named **GeoEduca**, aims to analyze and predict cutoff scores for PROUNI scholarships while incorporating geographic, socioeconomic, and institutional factors. By leveraging data science techniques, the project explores how location, tuition fees, and scholarship availability influence cutoff scores, and aims to provide insights into regional disparities and trends in higher education accessibility.

# Project Objectives

- **Cutoff Score Prediction**: Build a machine learning model to predict cutoff scores for scholarships (full and partial, with and without quotas).

- **Geographical Insights**: Explore and visualize how geographic factors (region, state, city) influence cutoff scores and access to higher education.

- **Institutional Analysis**: Investigate how course attributes (tuition fees, availability of scholarships, and shift schedules) impact scores.

- **Regional Disparities**: Identify patterns and disparities in cutoff scores and scholarship distribution across different regions of Brazil.

- **Integration with Institutional Data**: Incorporate external datasets with geographic and institutional details (e.g., addresses, neighborhood characteristics) to enhance analysis.

## Dataset Description
The dataset for this project is sourced from **Brazil’s Ministry of Education (MEC)** and consists of the following:

### Primary Dataset: PROUNI Scholarships (2018)

**Key Features**:

- **degree_level** (e.g., Bachelor’s, Associate’s)

- **shift** (e.g., Full-time, Nighttime)

- **tuition** (monthly fee in BRL)

- **scholarships_full** (number of full scholarships available)

- **scholarships_partial** (number of partial scholarships available)

- **cutoff_score_full** (cutoff score for full scholarships)

- **cutoff_score_partial** (cutoff score for partial scholarships)

- **course_name** (e.g., Medicine, Nursing)

- **campus_location** (city and state of the university)

### Secondary Dataset: Institutional Addresses

**Key Features**:

- **state, city, street, neighborhood**

- **institution_contact** (e.g., phone, external ID)

## Data Cleaning and Integration:

Ensure consistency in location data between datasets.

Merge datasets on university and campus information for geographic analysis.

## Tools and Technologies
- **Programming Language**: Python

- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

- **Visualization**: Dashboards using Plotly/Folium for geographic insights

## Machine Learning Models:
- **Regression** (for predicting cutoff scores)
- **Classification** (e.g., likelihood of receiving a scholarship)

## Pipeline

1. Data Loading and Cleaning: 
    - Load the primary and secondary datasets.
    - Handle missing values and normalize numerical features (e.g., tuition).

2. Exploratory Data Analysis (EDA):
    - Visualize distribution of cutoff scores by region and course.
    - Analyze correlation between tuition fees, scholarships, and cutoff scores.

3. Feature Engineering:
    - Create new features such as regional averages and tuition-to-scholarship ratios.
    - Incorporate geographic clustering (e.g., regions, city population).

4. Model Development:
    - Train regression models to predict cutoff scores.
    - Evaluate model performance (e.g., MAE, RMSE).

5. Visualization:
    - Develop dashboards/maps to present geographic insights.

## Documentation and Reporting:

Summarize findings, including regional disparities and predictive accuracy.

## Potential Use Cases

- Policymakers can use insights to improve scholarship allocation strategies and address regional disparities.

- Universities can optimize course offerings and scholarship distributions to attract more students.

- Students can leverage predictive models to evaluate their likelihood of receiving a scholarship.

## Next Steps

Refine predictive models by incorporating additional features such as socioeconomic data.

Expand geographic analysis with external data (e.g., city demographics, economic indices).

Share findings through an interactive dashboard for public use.

## Contributors

If you would like to contribute or have questions, feel free to reach out!