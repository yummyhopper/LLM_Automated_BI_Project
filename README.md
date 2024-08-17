# Chatting With A BigQuery Database Using LLMs: A New Frontier For BI?

![](automated_BI.webp)

### Introduction

Imagine your database as a person—let's call him Kregg. Kregg is an ordinary individual, except he possesses all your business analytics at his fingertips. Whenever you have a question about your data, you simply ask Kregg, and he provides the answer. The goal of this project was to create a chatbot that enables business executives to interact with their data through natural language. To achieve this, I developed an AI application using LangChain that queries a public BigQuery e-commerce database, allowing direct interaction with the data via a Gradio interface. The process began by installing and importing the necessary packages and libraries, setting up BigQuery credentials, and cloning the database. I then defined functions to extract schema information from the database, including nested fields, and generated a natural language description to input into the model. Using this schema, the model generates SQL queries based on user questions, returning a dataframe with the requested data. Additionally, I developed a chat interface that enables users to ask questions and extract insights from the data, along with a graphing agent for data visualizations. This project represents a new frontier for business intelligence, empowered by large language models. While the SQL isn't always perfect and the chatbot occasionally encounters challenges, the ability to execute queries on a personal database significantly accelerates the business intelligence workflow and introduces innovative ways to interact with data.

### Use Cases

The "Kregg" project represents an innovative approach to business intelligence by enabling natural language interaction with a database through a chatbot interface. Designed to assist business executives, Kregg allows users to ask questions about their data and receive immediate, actionable insights without needing to write SQL queries or understand the underlying database structure. For instance, executives can quickly ascertain their total sales for the last quarter, analyze customer acquisition trends, and identify low-stock products simply by asking Kregg. This capability significantly enhances operational efficiency, making it easy to track inventory levels, evaluate marketing campaign ROI, and generate financial reports on demand.

Moreover, Kregg facilitates customer support analytics by providing data on ticket resolution times and helps in identifying sales trends over time. By making data more accessible and reducing the reliance on technical teams, Kregg empowers non-technical users to generate custom reports, track budget expenditures, and optimize operational workflows. The project leverages the power of large language models and integrates them with a Gradio interface, ensuring that business executives can interact with their data in a conversational manner. This not only speeds up the business intelligence workflow but also opens up new ways to interact with data, ultimately driving more informed decision-making and strategic planning. Despite some limitations, such as occasional inaccuracies in SQL generation, the benefits of having real-time, easy-to-access data insights far outweigh the drawbacks, marking a significant advancement in the field of business intelligence.

### System Prompt

Developing the "Kregg" project required meticulous prompt engineering to achieve successful execution. One of the major challenges was ensuring the accurate generation of SQL queries. Since the model needed to interact with a public BigQuery ecommerce database, it was crucial to ensure that the SQL it generated was clean and correctly formatted. This involved extensive fine-tuning and testing of the prompts to ensure that they could handle various user queries and return precise, well-structured SQL code. Proper SQL generation was essential to maintain the integrity of the data retrieved and to provide reliable insights to the users.

In addition to generating accurate SQL, another significant aspect of the project was designing the chatbot's conversational prompt. I aimed to create an engaging and entertaining user experience by making the interactions with Kregg more conversational and humorous. This required a different approach to prompt engineering, focusing on natural language processing and user engagement. The conversational prompt needed to present facts in a way that was both informative and enjoyable, making the process of querying data feel less like a technical task and more like a friendly conversation.

Balancing these two aspects—technical accuracy and conversational engagement—was key to the project's success. The SQL prompt needed to be precise and robust to handle complex queries and return correct results. Meanwhile, the conversational prompt aimed to make the user experience more enjoyable and accessible, encouraging users to interact with their data more frequently and intuitively. This dual approach not only enhanced the usability of the system but also made the interaction with business data more dynamic and user-friendly.

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
