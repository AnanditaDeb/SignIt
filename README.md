# Sign It
Bridging Communication Gaps Through Sign Language Recognition
Sign It is a machine-learning-based web application designed to increase accessibility for the deaf and hard-of-hearing community. Utilizing advanced algorithms and machine learning, it provides real-time ASL and ISL (American Sign Language, Indian Sign Language) translation and interactive ASL and ISL learning modules, empowering users to interact seamlessly with both hearing and non-hearing communities.

# Project Overview
Sign language is a vital communication method, yet it remains unfamiliar to many people. For the deaf and hard-of-hearing, communicating in a predominantly hearing world can be challenging. Sign It aims to bridge this gap by offering real-time ASL translation and interactive ASL learning, catering specifically to the needs of the hearing-impaired community.

## Key features:

- **Real-Time Translation**: Converts audio into ASL, facilitating accessible communication.
- **Interactive Learning Modules**: Engages users in ASL learning to foster inclusivity.
- **Data Integration Pipeline**: An ETL pipeline in Airflow efficiently manages data ingestion, transformation, and storage for optimized performance.

## Documentation
Access the detailed project documentation here.

Application Links
Streamlit Interface: Sign It Web App
FastAPI Documentation: API Documentation
Airflow Dashboard: Airflow Management

## Tech Stack
- **Backend**: FastAPI
- **Frontend**: Streamlit
- **ML Frameworks**: Mediapipe, Vertex AI
- **Data Management**: Docker, AWS S3
- **Orchestration and Monitoring**: Airflow, Docker 
- **Analytics and Visualization**: Tableau

## Project Execution

### Prerequisites
To begin, ensure that you have the following installed:

- Docker Desktop (Install Docker)
- Python (v3.8 or higher)
- Kaggle API for dataset access


### Setup Instructions
- Clone the Repository

- Environment Variables Create a .env file in the project root with the following environment variables:

AIRFLOW_UID=<your_airflow_uid>
AIRFLOW_GID=<your_airflow_gid>
AIRFLOW_USERNAME=<your_airflow_username>
AIRFLOW_PASSWORD=<your_airflow_password>
AIRFLOW_URL=<your_airflow_url>

AWS_ACCESS_KEY=<your_aws_access_key>
AWS_SECRET_KEY=<your_aws_secret_key>
Sign It_BUCKET=<your_s3_bucket_name>

OPENAI_SECRET_KEY=<your_openai_secret_key>
API_URL=<api_url>
JWT_SECRET_KEY=<jwt_secret_key>

- Run Docker Containers Build and run the necessary Docker containers with the following commands:

docker-compose build
docker-compose up -d
Note: Ensure Docker Desktop is running before executing these commands.

### Folder Structure
The project is organized as follows:

Sign It/
│
├── streamlit/      # Contains web application files
├── api/            # FastAPI functions for backend API
├── pytest/         # Testing files and use cases
├── data/           # Dataset, ASL videos, and images
├── ml-model/       # Code to use the mediapipe gesture recognition model
├── airflow/        # Airflow DAGs for data processing
└── .env            # Environment variables file

![Architecture Diagram](image.png)

