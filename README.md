🚀 MLOps Project: End-to-End Machine Learning Pipeline

📌 Overview

This project demonstrates a complete MLOps pipeline, integrating various tools and technologies to streamline the machine learning lifecycle. From data ingestion to deployment, it follows best practices in automation, version control, monitoring, and CI/CD.

🔥 Key Features

✅ Project Template Automation – Automated project setup using Python scripts.

✅ Virtual Environment & Dependency Management – Uses Conda & requirements.txt for reproducibility.

✅ MongoDB Atlas for Data Storage – Cloud-based NoSQL database for scalable storage.

✅ Data Pipeline & Preprocessing – Includes ingestion, validation, transformation.

✅ Model Training & Evaluation – Implements robust training pipeline with automated evaluation.

✅ AWS Integration – Uses AWS S3 for model storage and IAM for secure access.

✅ CI/CD with GitHub Actions & Docker – Automates model deployment.

✅ Model Deployment on EC2 – Hosts the ML model as an API using a self-hosted runner.

✅ Scalable & Secure – Implements best practices for security, monitoring, and performance.

📂 Project Structure

📁 mlops_project
│── 📂 data                 # Raw & processed data storage

│── 📂 models               # Trained models & artifacts

│── 📂 notebooks            # EDA & experiments

│── 📂 src                  # Core project code

│   ├── 📂 components       # Data ingestion, validation, transformation, training

│   ├── 📂 entity           # Configuration & model schema definitions

│   ├── 📂 configuration    # MongoDB & AWS connection setup

│   ├── 📂 pipelines        # End-to-end pipeline scripts

│   ├── 📂 utils            # Helper functions

│── 📄 app.py               # Flask API for model inference

│── 📄 Dockerfile           # Docker configuration

│── 📄 requirements.txt     # Required dependencies

│── 📄 setup.py             # Package setup

│── 📄 .github/workflows    # CI/CD configurations

🛠 Tech Stack

📊 Data Pipeline

Storage: MongoDB Atlas (NoSQL)

Processing: Pandas, NumPy

Validation: Custom schema validation

🤖 Model Training & Evaluation

Frameworks: Scikit-learn, TensorFlow, PyTorch

Hyperparameter Tuning: GridSearchCV

Model Storage: AWS S3 Bucket

⚙️ Deployment & Infrastructure

Cloud: AWS (S3, EC2, IAM, ECR)

Containerization: Docker

CI/CD: GitHub Actions

Web Framework: Flask

🚀 Setup & Execution

1️⃣ Clone the Repository

git clone https://github.com/your-repo/mlops-project.git
cd mlops-project

2️⃣ Set Up Virtual Environment & Install Dependencies

conda create -n vehicle python=3.10 -y
conda activate vehicle
pip install -r requirements.txt

3️⃣ Configure MongoDB Atlas

Sign up & create a MongoDB cluster

Add your IP (0.0.0.0/0) for unrestricted access

Copy the connection string & replace <username>:<password> in MONGODB_URL

4️⃣ Configure AWS Credentials

export AWS_ACCESS_KEY_ID="your-key-id"
export AWS_SECRET_ACCESS_KEY="your-secret-key"
export AWS_DEFAULT_REGION="us-east-1"

5️⃣ Run the Project

python app.py

6️⃣ Deploy Using Docker & CI/CD

Dockerize the project using Dockerfile

Push to AWS ECR & deploy to EC2

docker build -t mlops-project .
docker tag mlops-project:latest <AWS_ECR_REPO_URI>:latest
docker push <AWS_ECR_REPO_URI>:latest

📌 CI/CD Pipeline

✅ GitHub Actions automates testing, building, and deploying.

✅ Self-hosted Runner on AWS EC2 ensures scalability.

✅ AWS ECR stores the Docker image, while AWS EC2 serves the application.

CI/CD Workflow

Push Code to GitHub → Triggers GitHub Actions workflow

Build & Test → Runs unit tests and quality checks

Docker Build & Push → Image stored in AWS ECR

Deploy to EC2 → Pulls latest image and restarts the container

🌟 Future Enhancements

🔹 Monitoring & Logging – Implement AWS CloudWatch or Prometheus.

🔹 Model Retraining Pipeline – Automate data drift detection & retraining.

🔹 Feature Store – Use Feast for managing ML features.

🤝 Contributing

Contributions are welcome! Feel free to open issues and submit PRs.

📞 Contact

📧 Email: ruzsanbhadha@gmail.com 

🔗LinkedIn: https://www.linkedin.com/in/ruzsan-bhadha-99253588/

📁 GitHub: https://github.com/ruzan-ai/MLops_proj1

🚀 If you found this project helpful, don't forget to ⭐ the repo!

