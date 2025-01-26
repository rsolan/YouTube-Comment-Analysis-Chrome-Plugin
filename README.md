# YouTube Comment Sentiment Analysis Chrome Plugin with MLflow and AWS

## Description:

Developed a Chrome extension that provides real-time sentiment analysis of YouTube comments, offering influencers valuable insights into audience engagement and feedback. The project integrates advanced machine learning tools and DevOps practices to ensure scalability and seamless deployment.

The project leveraged a machine learning pipeline with MLflow for experiment tracking and DVC for managing datasets and model versions, ensuring reproducibility. A Flask API served as the backend, while the frontend was built using JavaScript for seamless integration with YouTube. The machine learning models, trained using SVM and XGBoost, were registered and deployed using a Docker application, and the deployment process was automated via CI/CD pipelines. The application was hosted on AWS EC2, with Auto Scaling Groups (ASG) for high availability and load balancing, while AWS CodeDeploy facilitated smooth rolling updates during deployment. The entire system was optimized for efficiency with continuous integration, tracking, and automated deployment, ensuring scalability and ease of maintenance.




## Highlights:

MLflow for Experiment Tracking: Utilized MLflow to track machine learning experiments, enabling efficient model management and version control throughout the project lifecycle.

Model Deployment & CI/CD: Deployed sentiment analysis models using Flask API, integrated with a CI/CD pipeline to automate model deployment on AWS EC2 instances. Leveraged Docker for containerization and AWS ECR for image storage.

DVC Pipeline Integration: Managed datasets and model versions through DVC, ensuring reproducibility and consistency across development and production environments.

Scalable Deployment on AWS: Configured an Auto Scaling Group (ASG) with two EC2 instances for load balancing and fault tolerance. Implemented deployment strategies using AWS CodeDeploy with rolling updates for zero-downtime deployments.

Frontend with JavaScript: Designed the user-facing component as a Chrome extension using JavaScript, offering users real-time sentiment insights directly on YouTube.

CI Flow Automation: Streamlined the CI/CD flow for automated pipeline execution, ensuring continuous delivery and integration of updates with minimal manual intervention.


This project demonstrates expertise in machine learning model tracking, pipeline management, and automated deployment, offering scalable and reliable insights for YouTube content creators.


# Full-Stack Chrome Extension for Real-Time Sentiment Analysis on YouTube Comments

## 🚀 Technologies

- **Frontend:** HTML, CSS, JavaScript
- **Backend:** Flask, Python
- **Machine Learning:** scikit-learn, XGBoost
- **Version Control:** DVC (Data Version Control)
- **Containerization:** Docker
- **Cloud Services:** AWS (EC2, S3, CodePipeline, CodeDeploy)
- **MLOps:** MLflow

## 📃 Objective

This project aims to develop a full-stack Chrome extension that provides **real-time sentiment analysis** for **YouTube comments**. The tool helps **influencers** and **content creators** gain actionable insights into audience engagement by classifying comments as **positive**, **negative**, or **neutral**. It combines **frontend interactivity** with **machine learning pipelines** to deliver a scalable and efficient sentiment classification system.

## 💡 Overview

This project integrates a **Chrome extension** (user-facing frontend) with a backend powered by **machine learning models** and **cloud services**. It enables seamless, real-time sentiment analysis of comments on YouTube videos. Comments are classified into three categories: **positive**, **negative**, or **neutral**.

## 🔧 Key Features & Contributions

### Frontend Development

- Developed a **user-friendly Chrome extension** interface using **HTML**, **CSS**, and **JavaScript**.
- Integrated **APIs** to provide **real-time sentiment predictions**.
- Ensured responsive design elements for optimal usability across different devices.

### Backend Development

#### Machine Learning Models

- Built and evaluated **sentiment classification models** using **LightGBM**, achieving **87% accuracy** and an **86 F1-score**.
- Guided model improvements with **precision**, **recall**, and **F1-score** metrics.

#### Flask-based RESTful API

- Developed a **Flask-based REST API** to process user requests and return sentiment analysis results.

### End-to-End Machine Learning Pipeline

- Used **MLflow** to track experiments and model performance, ensuring reproducibility.
- Managed datasets and model versions with **DVC (Data Version Control)** for collaboration and updates.

### Deployment

#### Containerization & Orchestration

- **Dockerized** the backend to ensure consistent deployment across different environments.

#### Cloud Deployment

- Hosted the backend on **AWS EC2** instances.
- Utilized **S3** for storage, and **CodePipeline** and **CodeDeploy** for CI/CD automation.
- Implemented **Auto Scaling Groups (ASG)** to handle varying traffic.

### Performance Optimization

- Optimized API and server performance for **fast response times** and seamless user experience.

## 🏆 Achievements

- Integrated a **scalable, real-time sentiment analysis system** into a Chrome extension, showcasing skills in full-stack development, machine learning, and cloud deployment.
- Achieved **99.34% accuracy** in sentiment classification models.
- Streamlined deployment using **MLflow** and **DVC**, ensuring an efficient and reproducible ML pipeline.

## 🎯 Goals Achieved

- Bridged the gap between **machine learning** and **user-friendly application design**.
- Empowered **content creators** to make **data-driven decisions** for content optimization.
- Demonstrated expertise in building **scalable, full-stack ML solutions** with cloud deployment and **CI/CD** practices.

## 🌱 Potential Applications

- **Content Creators:** Analyze audience sentiment trends for content strategy.
- **Researchers:** Study online sentiment and behavior patterns in social media.
- **Businesses:** Leverage sentiment data for marketing and engagement strategies.

## ⚙️ Future Improvements

- Explore **transformer-based models** for more advanced sentiment analysis and context understanding.
- Extend the tool to other platforms like **Instagram** or **Twitter**.
- Develop a **dashboard** to visualize sentiment trends and audience engagement over time.



Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
