# Chatting With A BigQuery Database Using LLMs: A New Frontier For BI?

### Description

Imagine if your database was a person... Let's call him Kregg. Kregg is a normal guy other than having your entire database of business analytics at his finger tips. If you have a question about your data, you can just ask Kregg and he'll tell you the answer. 

The goal of this project was to build a chatbot that could facilitate a discussion between a business executive and their data through natural language. I used LangChain to build an AI application that queries a public BigQuery ecommerce database, and then allows you to chat directly with your data through a Gradio interface.

I began by installing and importing the necessary packages and libraries, setting up my BigQuery credentials, and cloning the database. I then by defining functions that scraped the schema information from the database, including nested fields, and built a description in natural language that I could feed to the model. Using the schema the model then writes a SQL query based on the users question and returns a dataframe with the data as an answer. I then created a chat interface where users can ask questions and extract insights from the data and a graphing agent for data visualizations.

This project presents a new frontier for business intelligence enabled by large language models. While the SQL isn't always flawless and the chatbot can get confused at times, the ability to run and execute queries on a personal database dramatically speeds up the business intelligence workflow and presents new ways to interact with data.

### Use Cases

The "Kregg" project represents an innovative approach to business intelligence by enabling natural language interaction with a database through a chatbot interface. Designed to assist business executives, Kregg allows users to ask questions about their data and receive immediate, actionable insights without needing to write SQL queries or understand the underlying database structure. For instance, executives can quickly ascertain their total sales for the last quarter, analyze customer acquisition trends, and identify low-stock products simply by asking Kregg. This capability significantly enhances operational efficiency, making it easy to track inventory levels, evaluate marketing campaign ROI, and generate financial reports on demand.

Moreover, Kregg facilitates customer support analytics by providing data on ticket resolution times and helps in identifying sales trends over time. By making data more accessible and reducing the reliance on technical teams, Kregg empowers non-technical users to generate custom reports, track budget expenditures, and optimize operational workflows. The project leverages the power of large language models and integrates them with a Gradio interface, ensuring that business executives can interact with their data in a conversational manner. This not only speeds up the business intelligence workflow but also opens up new ways to interact with data, ultimately driving more informed decision-making and strategic planning. Despite some limitations, such as occasional inaccuracies in SQL generation, the benefits of having real-time, easy-to-access data insights far outweigh the drawbacks, marking a significant advancement in the field of business intelligence.

### System Prompt

Developing the "Kregg" project required meticulous prompt engineering to achieve successful execution. One of the major challenges was ensuring the accurate generation of SQL queries. Since the model needed to interact with a public BigQuery ecommerce database, it was crucial to ensure that the SQL it generated was clean and correctly formatted. This involved extensive fine-tuning and testing of the prompts to ensure that they could handle various user queries and return precise, well-structured SQL code. Proper SQL generation was essential to maintain the integrity of the data retrieved and to provide reliable insights to the users.

In addition to generating accurate SQL, another significant aspect of the project was designing the chatbot's conversational prompt. I aimed to create an engaging and entertaining user experience by making the interactions with Kregg more conversational and humorous. This required a different approach to prompt engineering, focusing on natural language processing and user engagement. The conversational prompt needed to present facts in a way that was both informative and enjoyable, making the process of querying data feel less like a technical task and more like a friendly conversation.

Balancing these two aspects—technical accuracy and conversational engagement—was key to the project's success. The SQL prompt needed to be precise and robust to handle complex queries and return correct results. Meanwhile, the conversational prompt aimed to make the user experience more enjoyable and accessible, encouraging users to interact with their data more frequently and intuitively. This dual approach not only enhanced the usability of the system but also made the interaction with business data more dynamic and user-friendly.

### Data

- Pre-requisites: OpenAI API Key, Google BigQuery Service Account Credentials, and necessary packages (python-dotenv, langchain, langchain-openai, langchain_core, langchain_experimental google-cloud-bigquery, gradio).
- Data: https://developers.google.com/analytics/bigquery/web-ecommerce-demo-dataset?ref=rabbitmetrics.com
