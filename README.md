# On the Road Car Insurance - Predicting Claims

## Overview

This project aims to build a predictive model for **On the Road Car Insurance** to estimate whether a customer will make a claim during the policy period. The dataset provided consists of various customer attributes such as age, gender, income, driving experience, and more. The goal is to identify the **single feature** that results in the most accurate prediction of a customer's likelihood to make a claim.

## Dataset

The dataset used for this project is provided in a CSV file called `car_insurance.csv`. It contains anonymized customer data with several attributes:

| Column            | Description                                                      |
|-------------------|------------------------------------------------------------------|
| `id`              | Unique client identifier                                         |
| `age`             | Age group (16-25, 26-39, 40-64, 65+)                             |
| `gender`          | Client's gender (0: Female, 1: Male)                             |
| `driving_experience` | Client's years of driving experience (0-9, 10-19, 20-29, 30+)  |
| `education`       | Client's education level (No education, High school, University)  |
| `income`          | Client's income level (Poverty, Working class, Middle class, Upper class) |
| `credit_score`    | Client's credit score (between 0 and 1)                          |
| `vehicle_ownership`| Client's vehicle ownership status (0: Does not own, 1: Owns)     |
| `vehicle_year`    | Year of vehicle registration (0: Before 2015, 1: 2015 or later)  |
| `married`         | Client's marital status (0: Not married, 1: Married)             |
| `children`        | Number of children                                               |
| `postal_code`     | Client's postal code                                              |
| `annual_mileage`  | Number of miles driven annually                                   |
| `vehicle_type`    | Type of car (0: Sedan, 1: Sports car)                            |
| `speeding_violations`| Total number of speeding violations                           |
| `duis`            | Number of driving under the influence charges                    |
| `past_accidents`  | Number of previous accidents                                     |
| `outcome`         | Whether the client made a claim (0: No claim, 1: Made a claim)    |

## Objective

The objective of this project is to:

- Perform exploratory data analysis (EDA) to understand the relationships between features and the `outcome`.
- Build simple machine learning models for each individual feature.
- Evaluate which single feature results in the best performing model as measured by **accuracy**.

## Project Structure

```bash
.
├── data/
│   └── car_insurance.csv   # The dataset used for the analysis.
├── src/
│   ├── eda.py              # Exploratory Data Analysis (EDA) scripts.
│   ├── model.py            # Machine learning models to predict claim outcome.
├── README.md               # This readme file.
└── requirements.txt        # Python dependencies for the project.
```

## Steps

1. **Exploratory Data Analysis (EDA)**:
   - Analyze the distribution of features.
   - Visualize the correlation between customer attributes and `outcome`.

2. **Modeling**:
   - Build individual models using each feature.
   - Compare the models based on **accuracy**.

3. **Feature Selection**:
   - Identify the single most important feature for predicting the `outcome`.

## Dependencies

Install the required dependencies using the following command:

```bash
pip install -r requirements.txt
```

## How to Run

1. Clone this repository:

```bash
git clone https://github.com/yourusername/car-insurance-claims.git
```

2. Navigate to the project directory:

```bash
cd car-insurance-claims
```

3. Run the exploratory data analysis:

```bash
python src/eda.py
```

4. Train the models and evaluate accuracy:

```bash
python src/model.py
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

Happy modeling!
