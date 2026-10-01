# Machine Learning Zoomcamp

This repository documents my progress through [DataTalks.Club's Machine Learning Zoomcamp](https://github.com/DataTalksClub/machine-learning-zoomcamp), a hands-on course covering the development, evaluation, and deployment of machine learning systems. I am using this repository to organize my coursework, datasets, notebooks, scripts, and projects as I progress through the 2026 cohort. The repository follows the course structure, progressing from fundamental machine learning concepts and classical models to deep learning, model deployment, and production-oriented infrastructure.

## Course Overview

Machine Learning Zoomcamp is an applied machine learning engineering course covering the end-to-end machine learning workflow: **problem definition, data preparation, exploratory analysis, feature engineering, model training, evaluation, model selection, deployment, and serving**.

The course begins with supervised learning and progressively develops more advanced modelling and engineering skills, moving from regression and classification to ensemble methods and deep learning. Later modules focus increasingly on turning trained models into reproducible, accessible, and scalable services using APIs, containers, cloud infrastructure, serverless computing, and Kubernetes.

---

# Curriculum and Projects

## 1. Introduction to Machine Learning

The first module establishes the conceptual and technical foundations for the rest of the course.

Topics include:

* The machine learning workflow, supervised learning, regression, classification, and model selection
* The CRISP-DM framework and the distinction between training, validation, and deployment
* Python data-science foundations using **NumPy** and **pandas**, including vectors, matrices, data manipulation, and basic linear algebra

This provides the foundation for working with real-world datasets and building reproducible machine learning workflows.

---

## 2. Machine Learning for Regression

The module introduces regression through a car price prediction example, using it to demonstrate the end-to-end process of preparing a real-world dataset, developing a baseline model, evaluating predictions, and improving model performance.

Topics include:

* Data preparation, exploratory data analysis, validation strategies, and baseline modelling
* Linear regression from both mathematical and implementation perspectives, including vector/matrix formulations and the normal equation
* RMSE-based evaluation, feature engineering, categorical variables, regularization, and model tuning
* Using a final trained model to generate predictions on new observations

This module provides a foundation in both the mathematical principles behind regression and their practical implementation with Python and scikit-learn. ([02-regression](https://github.com/DataTalksClub/machine-learning-zoomcamp/tree/main/02-regression#readme))

---

## 3. Machine Learning for Classification

The third module extends the regression workflow to binary classification, using customer churn as the primary instructional example.

Topics include:

* Data preparation, exploratory analysis, validation, and categorical feature encoding using one-hot encoding
* Feature importance through churn rates, risk ratios, mutual information, and correlation
* Logistic regression, including probability-based predictions, classification thresholds, model training, and coefficient interpretation
* Generating predictions for new observations and translating customer data into predictive features

This module develops practical experience framing business questions as classification problems and working with both categorical and numerical predictors. ([03-classification](https://github.com/DataTalksClub/machine-learning-zoomcamp/tree/main/02-classification#readme))

---

## 4. Evaluation Metrics for Classification

The fourth module develops a more rigorous approach to evaluating classification models, moving beyond accuracy to metrics that distinguish different types of prediction errors.

Topics include:

* Confusion matrices, accuracy, precision, recall, and F1 score
* Classification thresholds and the trade-off between false-positive and false-negative predictions
* ROC curves, ROC AUC, and comparison of classifier performance
* Cross-validation and more robust approaches to model selection

The focus is on understanding which evaluation metrics are appropriate for a particular problem and how model performance changes under different decision thresholds.
([04-evaluation](https://github.com/DataTalksClub/machine-learning-zoomcamp/tree/main/04-evaluation#readme))

---

## 5. Deploying Machine Learning Models

This module moves from developing models in notebooks to building a **usable machine learning service**.

Topics include:

* Saving and loading trained models, transforming exploratory notebooks into reusable training scripts, and creating reproducible scikit-learn pipelines
* Python environment and dependency management with **uv**
* Building a **FastAPI** prediction service with input validation using **Pydantic**
* Packaging the application with **Docker** and deploying it to the cloud

Through this work, I’ll gain experience with the engineering practices required to take a trained model beyond experimentation and make it accessible through an API. The current course workshop uses FastAPI, uv, Docker, and Fly.io as the modern deployment stack. 
([05-deployment](https://github.com/DataTalksClub/machine-learning-zoomcamp/tree/main/05-deployment#readme))

---

## 6. Decision Trees and Ensemble Learning

The sixth module expands beyond linear models to explore non-linear models and ensemble methods for structured data.

Topics include:

* Decision trees, tree-based splitting, model interpretation, overfitting, and hyperparameter tuning
* Random forests and ensemble learning, including feature importance and aggregation across multiple trees
* Gradient boosting and **XGBoost**, including learning-rate, tree-depth, and iteration tuning

I’ll apply these techniques to a **credit risk scoring** problem and compare different tree-based approaches for tabular data.
([06-trees](https://github.com/DataTalksClub/machine-learning-zoomcamp/tree/main/06-trees#readme))

---

# Midterm Project

The midterm brings together the modelling and engineering techniques covered in the first six modules through an independent **end-to-end machine learning project**.

Through this project, I’ll:

1. Define a prediction problem and identify an appropriate dataset.
2. Explore and prepare the data.
3. Engineer relevant features and establish a validation strategy.
4. Train, evaluate, and tune multiple candidate models.
5. Select and serialize a final model.
6. Build a prediction service and deploy it.

The project topic is not yet selected and will be developed as the course progresses.

**Project:** [Midterm Project](./midterm-project/)

---

## 8. Neural Networks and Deep Learning

The eighth module transitions from classical machine learning to **deep learning**, using image classification as the primary application.

Topics include:

* Neural-network architecture, activation functions, loss functions, optimization, and training
* Image preprocessing, datasets and DataLoaders, and convolutional neural networks (CNNs)
* Transfer learning with pre-trained image models, including freezing layers, replacing classification heads, and fine-tuning
* Regularization, data augmentation, learning-rate tuning, model checkpointing, and model export

The current course materials include a PyTorch-based workshop, providing practical experience with modern deep-learning workflows alongside the underlying concepts. 
([08-deep-learning](https://github.com/DataTalksClub/machine-learning-zoomcamp/tree/main/08-deep-learning#readme))

---

## 9. Serverless Deep Learning

This module introduces **serverless cloud infrastructure** as another approach to deploying machine learning models.

Topics include:

* **AWS Lambda** for on-demand model inference
* Packaging machine learning models and dependencies for serverless execution
* **AWS API Gateway** for exposing prediction functionality through HTTP endpoints
* Deploying different types of models, including scikit-learn and deep-learning models

The module builds on the earlier deployment work while introducing the practical considerations of running machine learning workloads in a serverless environment.
([09-serverless](https://github.com/DataTalksClub/machine-learning-zoomcamp/tree/main/09-serverless#readme))

---

## 10. Kubernetes and TensorFlow Serving

The final core module explores **container orchestration and scalable model serving**.

Topics include:

* **TensorFlow Serving** and architectures that separate model serving from application logic
* Multi-service applications with Docker Compose
* Kubernetes concepts including pods, deployments, services, and scaling
* Deploying machine learning services to **Amazon Elastic Kubernetes Service (EKS)**

This extends the deployment concepts introduced earlier from individual containers and cloud functions to infrastructure capable of managing and scaling multiple services.
([10-kubernetes](https://github.com/DataTalksClub/machine-learning-zoomcamp/tree/main/10-kubernetes#readme))

---

# Capstone Projects

The capstone projects provide an opportunity to consolidate the machine learning and engineering skills developed throughout the course through larger independent projects.

## Capstone Project 1

For the first capstone, I’ll develop a complete machine learning system around an independently selected problem, demonstrating the ability to move from data and problem definition through modelling, evaluation, and deployment.

The project topic has not yet been selected.

**Project:** [Capstone Project 1](./capstone-project-1/)

## Capstone Project 2

A second independent capstone will provide an additional opportunity to apply the course's machine learning and deployment techniques to a different problem.

The project topic has not yet been selected.

**Project:** [Capstone Project 2](./capstone-project-2/)

The 2026 course requires two passing projects for the certificate: either the midterm and one capstone, or both capstones. Each project also includes peer review of other students' projects.

---

# Technical Skills

Throughout the course, I’ll develop practical experience with:

* **Programming & data:** Python, NumPy, pandas, Jupyter, data cleaning, EDA, and feature engineering
* **Machine learning:** scikit-learn, regression, classification, decision trees, random forests, gradient boosting, XGBoost, regularization, and hyperparameter tuning
* **Model evaluation:** validation strategies, regression and classification metrics, ROC AUC, confusion matrices, and cross-validation
* **Deep learning:** PyTorch, TensorFlow/Keras, CNNs, transfer learning, image preprocessing, and model optimization
* **ML engineering:** scikit-learn pipelines, model serialization, FastAPI, Pydantic, Docker, and reproducible environments
* **Cloud & infrastructure:** AWS Lambda, API Gateway, Kubernetes, TensorFlow Serving, and Amazon EKS

---

# Key Takeaways

By completing this course, I aim to demonstrate that I can work across the full lifecycle of a machine learning project rather than focusing solely on model training.

In particular, I’ll develop the ability to:

* **Translate real-world problems into machine learning problems**, selecting appropriate targets, features, validation strategies, and evaluation metrics.
* **Work independently with real-world datasets**, including data preparation, exploratory analysis, feature engineering, and categorical-data handling.
* **Develop and compare predictive models**, from interpretable linear and logistic regression through tree ensembles, gradient boosting, and neural networks.
* **Evaluate models critically**, understanding the trade-offs between different metrics, thresholds, validation strategies, and model configurations.
* **Build reproducible machine learning workflows**, moving from exploratory notebooks toward reusable training pipelines and serialized models.
* **Deploy models as usable services**, including API development, input validation, containerization, and cloud deployment.
* **Work with modern ML infrastructure**, including serverless computing, Kubernetes, and dedicated model-serving systems.
* **Complete end-to-end machine learning projects independently**, documenting decisions from problem definition through deployment.

My overall goal in this course is to develop not only an understanding of machine learning algorithms, but also the practical skills required to turn those algorithms into reliable, reproducible, and deployable machine learning systems.

