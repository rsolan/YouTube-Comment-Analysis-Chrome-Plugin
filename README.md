# YouTube Comment Sentiment Analysis Chrome Plugin with MLflow and AWS

## Description:

Developed a Chrome extension that provides real-time sentiment analysis of YouTube comments, offering influencers valuable insights into audience engagement and feedback. The project integrates advanced machine learning tools and DevOps practices to ensure scalability and seamless deployment.

The project leveraged a machine learning pipeline with MLflow for experiment tracking and DVC for managing datasets and model versions, ensuring reproducibility. A Flask API served as the backend, while the frontend was built using JavaScript for seamless integration with YouTube. The machine learning models, trained using SVM and XGBoost, were registered and deployed using a Docker application, and the deployment process was automated via CI/CD pipelines. The application was hosted on AWS EC2, with Auto Scaling Groups (ASG) for high availability and load balancing, while AWS CodeDeploy facilitated smooth rolling updates during deployment. The entire system was optimized for efficiency with continuous integration, tracking, and automated deployment, ensuring scalability and ease of maintenance.




## Key Highlights:

MLflow for Experiment Tracking: Utilized MLflow to track machine learning experiments, enabling efficient model management and version control throughout the project lifecycle.

Model Deployment & CI/CD: Deployed sentiment analysis models using Flask API, integrated with a CI/CD pipeline to automate model deployment on AWS EC2 instances. Leveraged Docker for containerization and AWS ECR for image storage.

DVC Pipeline Integration: Managed datasets and model versions through DVC, ensuring reproducibility and consistency across development and production environments.

Scalable Deployment on AWS: Configured an Auto Scaling Group (ASG) with two EC2 instances for load balancing and fault tolerance. Implemented deployment strategies using AWS CodeDeploy with rolling updates for zero-downtime deployments.

Frontend with JavaScript: Designed the user-facing component as a Chrome extension using JavaScript, offering users real-time sentiment insights directly on YouTube.

CI Flow Automation: Streamlined the CI/CD flow for automated pipeline execution, ensuring continuous delivery and integration of updates with minimal manual intervention.

## Technologies Used:

Machine Learning: SVM, XGBoost

Backend: Flask API

Experiment Tracking & Model Registry: MLflow, DVC

Containerization & Deployment: Docker, AWS ECR, EC2, CodeDeploy, Auto Scaling Groups (ASG)

Frontend: JavaScript (Chrome Extension)

CI/CD Automation: AWS CodePipeline, CodeDeploy

This project demonstrates expertise in machine learning model tracking, pipeline management, and automated deployment, offering scalable and reliable insights for YouTube content creators.

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
