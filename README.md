# 🛡️ Phishing Website Detection System using Machine Learning and MLOps

This project involves developing a machine learning system to predict whether a website is phishing or not. The system is designed to enhance cybersecurity by identifying and blocking malicious websites. The project integrates machine learning techniques with MLOps tools to create a scalable, automated, and efficient solution.

## 🚀 Project Overview

- **🎯 Objective:** Predict phishing websites using machine learning to improve cybersecurity.
- **🛠️ Key Technologies:** Python, Docker, AWS, MongoDB, FastAPI, GitHub Actions, MLflow, Airflow, Terraform.

## 🌟 Features

- **🔍 Machine Learning Model:** A model trained to detect phishing websites based on various indicators.
- **🔄 MLOps Pipeline:** Automated deployment pipeline using GitHub Actions, MLflow, Airflow, and Terraform.
- **⚙️ Scalable Deployment:** The system is deployed on AWS using Docker, and MongoDB, ensuring scalability and efficient management.
- **🌐 API Integration:** FastAPI is used to build and deploy APIs for interacting with the model.
- **💾 Database Integration:** MongoDB is used for storing and managing website data during model training and deployment.

## 🛠️ Installation and Setup

### Prerequisites
- 🐍 Python 3.8+
- 🐳 Docker
- ☁️ AWS account with necessary permissions
- 🍃 MongoDB


### 🖥️ Setup Virtual Environment
```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

### ⚙️ Configure AWS
- Ensure your AWS CLI is configured with the correct credentials.
- Update the `terraform/variables.tf` file with your AWS settings.

### 🚀 Deploy the System
1. **🐳 Build Docker Image:**
    ```bash
    docker build -t phishing-detection:v1 .
    ```
2. **📤 Push to AWS ECR:**
    Follow AWS ECR instructions to push your Docker image.
3. **🛠️ Run Terraform:**
    ```bash
    cd terraform
    terraform init
    terraform apply
    ```
## 🧑‍💻 Usage

1. **📊 Training the Model:**
    - Prepare your dataset and upload it to the specified MongoDB collection.
  
2. **🔍 Prediction:**
    - After deployment, the system will automatically predict whether new websites are phishing and store the results in MongoDB.
    - Interact with the model via APIs built with FastAPI.

## 📈 Results and Evaluation

- The model's performance metrics, such as accuracy, precision, and recall, are tracked using MLflow.

## 🤝 Contributing

If you'd like to contribute to this project, please fork the repository and use a feature branch. Pull requests are welcome.

## 📧 Contact

For any questions or feedback, please reach out to [Krishna Shukla](mailto:Kriishukla@gmail.com).
