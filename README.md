# 🚗 Car Price Prediction API

🎯 A production-ready Car Price Prediction API built with FastAPI and Scikit-Learn, featuring JWT authentication, Redis caching, Prometheus monitoring, Docker containerization, and deployment on Render.

## ✨ Features

* 🔐 JWT-based authentication and API key access
* 🚀 Machine Learning prediction endpoint powered by Scikit-Learn
* ⚡ Redis caching for faster repeated predictions
* 📊 Prometheus metrics for monitoring and observability
* 🛡️ Custom exception handling and request validation
* 🏗️ Modular and scalable project structure
* 🐳 Dockerized application for easy deployment
* ☁️ Deployed on Render with GitHub integration

## 🛠️ Tech Stack

* **Backend:** FastAPI, Pydantic
* **Machine Learning:** Scikit-Learn, Joblib
* **Authentication:** JWT (python-jose)
* **Caching:** Redis
* **Monitoring:** Prometheus
* **Containerization:** Docker
* **Deployment:** Render
* **Version Control:** Git & GitHub

## 📌 API Workflow

1. User sends a request to the prediction endpoint.
2. FastAPI validates the input using Pydantic models.
3. JWT authentication verifies the user.
4. Redis checks for cached predictions.
5. On a cache miss, the input is passed through the preprocessing pipeline and trained model.
6. The predicted car price is returned as a JSON response and stored in Redis for future requests.

## 🚀 Deployment

The application is containerized using Docker and deployed on Render for production use.

