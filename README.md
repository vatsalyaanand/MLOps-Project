# Building a Scalable MLOps CICD Pipeline

## Introduction

This project implements an end-to-end Machine Learning Operations (MLOps) pipeline, incorporating Continuous Ingestion and Continuous Deployment (CI/CD) pipelines to ensure scalability and efficiency. The workflow is designed to automate the machine learning lifecycle, from data ingestion and transformation to model deployment and updates.

Key features include:
- Modular coding for data ingestion, transformation, and model training.
- Integration of the machine learning model with a web front end using Flask, HTML, and CSS.
- Containerization of the application using Docker.
- Automated deployment to AWS using GitHub Actions, with updates triggered by changes to the main branch.

## Background

In modern cloud computing environments, transitioning from Jupyter Notebook or Google Colab to a scalable production setup is crucial. CI/CD pipelines automate the deployment process, reducing manual effort and costs while enabling continuous updates. This approach is utilized by major companies like Netflix and Facebook to streamline their deployment processes.

The project leverages several technologies:
- **Languages**: Python, HTML, CSS
- **Libraries**: 
  - **Pandas**: Data manipulation and analysis.
  - **NumPy**: Multi-dimensional arrays and matrices.
  - **Plotly**: Graphing library for publication-level graphs.
  - **Scikit-learn**: Tools for machine learning.
  - **Flask**: Micro web framework for building web applications.
- **Machine Learning Models**: The following ML models were utilized:
  - Linear Regression
  - K Neighbors Regressor
  - Decision Tree Regressor
  - Gradient Boosting Regressor
  - XG Boost Regressor
  - Cat Boost Regressor
  - Ada Boost Regressor
  - Random Forest Regressor
- **Docker**: Platform used for containerizing the application, ensuring consistent environments across development and production.
- **GitHub Actions**: Tool for automating the CI/CD pipeline, handling continuous integration, delivery, and deployment.
- **AWS ECR (Elastic Container Registry)**: Managed container image registry service used to store and manage Docker images.
- **AWS EC2 (Elastic Compute Cloud)**: Scalable virtual server service used for deploying and running the Docker container.

## Methods

1. **Project Setup**:
   - Created a GitHub repository for version control.
   - Set up Python 3.10 environment with required libraries.
   - Defined project structure with folders for data ingestion, transformation, model training, and pipelines.

2. **Data Handling**:
   - Used a student performance dataset for initial testing.
   - Performed data ingestion, transformation, and exploratory data analysis (EDA).

3. **Model Training**:
   - Implemented multiple machine learning models.
   - Conducted hyperparameter tuning and cross-validation.
   - Selected the best-performing model based on accuracy and R2 value.

4. **Web Application**:
   - Developed a web interface using Flask and HTML/CSS.
   - Implemented user input handling and prediction functionality.

5. **Containerization**:
   - Created a Dockerfile to build and containerize the application.

6. **CI/CD Deployment**:
   - Configured GitHub Actions for continuous integration, delivery, and deployment.
   - Utilized AWS services (ECR, EC2) for hosting and deploying the Docker container.

## Setup and Deployment

1. **Environment Setup**:
   - Clone the repository: `git clone https://github.com/vatsalyaanand/MLOps-Project`
   - Install dependencies: `pip install -r requirements.txt`

2. **Running Locally**:
   - Run the Flask application: `python app.py`

3. **Deployment**:
   - Build Docker image: `docker build -t Dockerfile .`
   - Push image to Amazon ECR.
   - Deploy on AWS EC2 using the configured Docker container.

4. **CI/CD Configuration**:
   - GitHub Actions are configured to automate the CI/CD process. Ensure AWS credentials are set in GitHub Secrets.


