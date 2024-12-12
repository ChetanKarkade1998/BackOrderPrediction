# Backorder Prediction for Supply Chain Optimization

## Description

This repository contains the analysis and code for predicting the likelihood of products going on backorder. The project leverages data preprocessing, exploratory data analysis, hypothesis testing, feature engineering, machine learning techniques, and deployment.

## Abstract

This project focuses on preprocessing, feature engineering, and machine learning techniques to predict the likelihood of products going on backorder. Using historical inventory data, a Random Forest model was developed and evaluated to classify backorder status. The solution emphasizes data cleaning, handling missing values, and balancing classes to improve model accuracy and reliability.

## Problem Statement

This project addresses the issue of backorders, which occur when a customer orders a product that is currently out of stock. The goal is to predict backorders using machine learning techniques to enhance inventory management efficiency and reduce associated business risks such as loss of sales, customer trust, and competitive edge.

## Objective

To develop a predictive model to classify products as being in backorder or not based on historical inventory data. The goal is to provide actionable insights for improving inventory management and reducing backorder-related issues.

## Data

The dataset used in this project is available on GitHub. It includes two files:

- `Kaggle_Training_Dataset_v2` (Training data)
- `Kaggle_Test_Dataset_v2` (Testing data)

The training data consists of 22 feature columns and one target column (`went_on_backorder`), which indicates whether a product went out of stock.

### Data Description

- **Target Variable**: `went_on_backorder` (binary: 1 for backorder, 0 for no backorder)
- **Features**: Various inventory and demand-related parameters like lead time, forecast group, sales group, etc.

## Project Workflow

1. **Data Source**: Collected historical supply chain data, including key metrics relevant to backorders.
2. **Data Analysis and Understanding**: Inspected the dataset for completeness and relevance. Performed exploratory data analysis to understand data distributions and relationships.
3. **Preprocessing**: Handled missing values and outliers. Performed feature engineering and selection to enhance predictive power.
4. **Data Interpretation**: Analyzed statistical correlations and identified key factors influencing backorders.
5. **Build Models**: Developed a Random Forest Classifier to predict potential backorders. Fine-tuned model hyperparameters for optimal performance.
6. **Data Evaluation**: Evaluated model performance using metrics like accuracy, precision, recall, and F1-score. Validated results with cross-validation techniques.
7. **Version Control**: Utilized GitHub for version control, allowing seamless collaboration and code management.
8. **Deployment**: Deployed the model using Docker to ensure scalable and reliable implementation. Incorporated CI/CD pipelines for efficient updates and maintenance. Used cloud services (e.g., AWS) to host the application and enable scalability.

## Files Overview

- **`FinalModelOnly.ipynb`**: Contains the implementation of the final machine learning model. Focuses on training, optimizing, and evaluating a model using selected features. Uses GPU acceleration for efficient computation.
- **`Final.ipynb`**: Includes a more detailed workflow leading up to the final model. Covers data preprocessing, exploratory data analysis, and initial model trials.
- **`Backorder.ipynb`**: A comprehensive notebook with documentation and step-by-step implementation. Includes markdown explanations for clarity. Demonstrates the full pipeline, including feature engineering and intermediate results.

## Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/backorder-prediction.git
   ```

2. **Navigate to the project directory:**
   ```bash
   cd backorder-prediction
   ```

3. **Install required dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the analysis:**
   Open and execute the Jupyter Notebooks located in the `notebooks/` directory:
   - `Backorder.ipynb`: Contains step-by-step analysis, from data preprocessing to model evaluation.
   - `Final.ipynb`: Focuses on data preprocessing and exploratory analysis.
   - `FinalModelOnly.ipynb`: Executes the final model for predictions.

## Key Results

- Identified key supply chain metrics influencing backorders.
- Achieved high model performance metrics (e.g., 90% accuracy, 0.85 F1-score).
- Provided actionable recommendations to optimize inventory management.

## Tools and Libraries

- **Programming and Analysis**: Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)
- **Data Management**: SQL for efficient storage and retrieval of data connections
- **Version Control**: GitHub for managing project versions and collaboration
- **Deployment**: Docker for scalable and reliable implementation, CI/CD pipelines for automated updates
- **Cloud Services**: AWS for hosting and scaling the application
- **Environment**: Jupyter Notebooks for interactive development and analysis

## Conclusion

The project successfully demonstrated the ability to predict backorders using historical supply chain data. By implementing advanced feature engineering, a Random Forest Classifier, and deploying the model with Docker and CI/CD pipelines, it provided a scalable solution for improving inventory management and minimizing disruptions. The use of cloud services like AWS ensures the application is scalable and reliable for real-world deployment. The insights derived from this analysis can help organizations better understand the factors contributing to backorders, enabling more informed decision-making.

## Future Work

- Explore additional machine learning algorithms, such as Gradient Boosting or Neural Networks, to further improve predictive performance.
- Incorporate real-time data streams to enable dynamic backorder predictions.
- Expand the analysis to include external factors, such as market trends or supplier reliability, to enhance the model's accuracy and applicability.
