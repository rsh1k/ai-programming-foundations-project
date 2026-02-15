# AI Programming Foundations: NYC Airbnb Analysis

## Project Description
This project implements a reproducible data science workflow to analyze the NYC Airbnb market. It covers the full pipeline from raw data ingestion and modular cleaning to exploratory statistical analysis and visualization. This foundational workflow ensures data integrity for future Agentic AI and Machine Learning implementations.

## What I Built
* A modular Python pipeline for data sanitization and outlier removal.
* An EDA suite that aggregates market trends by geographic borough.
* Visualizations including price distributions and attribute correlations.

## Dataset
**Name:** NYC Airbnb Open Data (2019)  
**Source:** [Kaggle Dataset Link](https://www.kaggle.com/dgomonov/new-york-city-airbnb-open-data)

## Bias Awareness
Poor data cleaning can introduce significant bias. For example, if we simply dropped all rows with missing values (Listwise Deletion), we might exclude newer hosts who have not yet received reviews, biasing the dataset toward established properties. [cite_start]In this project, I filled missing `reviews_per_month` values with `0` to ensure these new listings were still represented in the overall analysis[cite: 67].

## Future AI & ML Potential
This project serves as a professional, reusable foundation for several advanced AI applications:
* **ML Workflow Changes:** This clean dataset is prepared for training **Regression models** to predict listing prices based on geographic location and room type.
* **Neural Network Preparation:** The numerical features are ready for normalization, and categorical variables like 'Borough' can be one-hot encoded to serve as inputs for **Deep Learning** frameworks.
* **Agentic Automation:** This modular workflow could be converted into a tool for **Autonomous AI Agents** to ingest, clean, and analyze new market data automatically, ensuring consistent data quality without human intervention.

## How to Run the Project
1. Clone this repository.
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
	```
3. Open the Jupyter Notebook:
   ```jupyter notebook notebooks/data_workflow.ipynb```

