# Chatting With A BigQuery Database Using LLMs

![](automated_BI.webp)

### Introduction

Imagine your database as a person—let's call him Kregg. Kregg is an ordinary individual, except he possesses all your business analytics at his fingertips. Whenever you have a question about your data, you simply ask Kregg, and he provides the answer. The goal of this project was to create a chatbot that enables business executives to interact with their data through natural language. To achieve this, I developed an AI application using LangChain that queries a public BigQuery e-commerce database, allowing direct interaction with the data via a Gradio interface. The process began by installing and importing the necessary packages and libraries, setting up BigQuery credentials, and cloning the database. I then defined functions to extract schema information from the database, including nested fields, and generated a natural language description to input into the model. Using this schema, the model generates SQL queries based on user questions, returning a dataframe with the requested data. Additionally, I developed a chat interface that enables users to ask questions and extract insights from the data, along with a graphing agent for data visualizations. This project represents a new frontier for business intelligence, empowered by large language models. While the SQL isn't always perfect and the chatbot occasionally encounters challenges, the ability to execute queries on a personal database significantly accelerates the business intelligence workflow and introduces innovative ways to interact with data.

### Contents

The entire project is in the dashboards.ipynb file. This includes the code, explanations of the code, the results, written analysis of the prompt engineering, and a written analysis of possible use cases for this sort of project.

### Data

This dataset was obtained through the BigQuery Public Datasets program. It contains real sample data from the Google Merchandise Store, an online store ran by Google. The dataset is structured as a relational database in Google BigQuery. More information can be found here: https://developers.google.com/analytics/bigquery/web-ecommerce-demo-dataset

### Tools + Skills

- Prompt Engineering
- Google BigQuery
- Database Architecture
- Python
  - python-dotenv
  - langchain
  - langchain-openai
  - langchain_core
  - langchain_experimental
  - google-cloud-bigquery
  - gradio
