# Chatting With A BigQuery Database Using LLMs: A New Frontier For BI?

### Description

Imagine if your database was a person... Let's call him Kregg. Kregg is a normal guy other than having your entire database of business analytics at his finger tips. If you have a question about your data, you can just ask Kregg and he'll tell you the answer. 

The goal of this project was to build a chatbot that could facilitate a discussion between a business executive and their data through natural language. I used LangChain to build an AI application that queries a public BigQuery ecommerce database, and then allows you to chat directly with your data through a Gradio interface.

I began by installing and importing the necessary packages and libraries, setting up my BigQuery credentials, and cloning the database. I then by defining functions that scraped the schema information from the database, including nested fields, and built a description in natural language that I could feed to the model. Using the schema the model then writes a SQL query based on the users question and returns a dataframe with the data as an answer. I then created a chat interface where users can ask questions and extract insights from the data in various ways such as building reports or slide decks.

This project presents a new frontier for business intelligence enabled by large language models. While the SQL isn't always flawless and the chatbot can get confused at times, the ability to run and execute queries on a personal database dramatically speeds up the business intelligence workflow and presents new ways to interact with data.

### Use Cases

What kind of queries might a user enter and what are the responses the system should give

### System Prompt

What kind of system prompt etc is needed to make the LLM respond in the appropriate why, e.g. response length, style, when not to give an answer etc.

### Data

  Data: https://developers.google.com/analytics/bigquery/web-ecommerce-demo-dataset?ref=rabbitmetrics.com