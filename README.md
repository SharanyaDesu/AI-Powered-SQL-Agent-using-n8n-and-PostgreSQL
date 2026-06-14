# AI-Powered-SQL-Agent-using-n8n-and-PostgreSQL

This project demonstrates how an AI Agent can interact with a PostgreSQL database using natural language queries.
Instead of writing SQL manually, users can ask questions in plain English such as:

•	Show total sales for last month

•	What are the top 10 customers by revenue?

•	How many orders were placed this year?

The AI Agent understands the user's request, generates the appropriate SQL query, executes it against the PostgreSQL database, and returns the results.

The solution is built using n8n workflow automation and consists of two workflows, a Parent Workflow and a Child Workflow.

The Parent Workflow starts when a user sends a message through the chat interface. The message is passed to an AI Agent configured with a Gemini Chat Model and memory capabilities.

The AI Agent analyzes the user's question and generates the required SQL query. The SQL query is stored in a parameter and passed to a Child Workflow.

The Child Workflow is triggered by the Parent Workflow. It performs the following steps:

1.	Receives the SQL query from the Parent Workflow.
   
2.	Executes the query against the PostgreSQL database.
   
3.	Returns the query results back to the Parent Workflow.
   
4.	Displays the final response to the user.
   
# Workflow Process

1.	User asks a question in natural language.
   
2.	Chat message triggers the Parent Workflow.
   
3.	AI Agent interprets the question.
   
4.	AI Agent generates the SQL query.
   
5.	SQL query is passed to the Child Workflow.
    
6.	Child Workflow executes the query in PostgreSQL.
    
7.	Query results are returned to the Parent Workflow.
    
8.	User receives the answer in a conversational format.

    
# Technologies Used

•	n8n

•	Gemini Chat Model

•	PostgreSQL

•	AI Agent

•	Workflow Automation

•	Natural Language Processing (NLP)

# Features

•	Natural language to SQL conversion

•	Automated query execution

•	PostgreSQL integration

•	Parent and Child workflow architecture

•	AI-powered data retrieval

•	Conversational user experience

# Architecture

The workflow architecture diagram is included in this repository for reference.

# Parent Workflow
<img width="1500" height="527" alt="Workflow_1" src="https://github.com/user-attachments/assets/34406cd5-84e2-4329-8207-16bc400959f1" />


# Child Workflow
<img width="910" height="272" alt="Workflow_2" src="https://github.com/user-attachments/assets/01b1f9be-3433-4e70-bbd7-416e3e39b947" />



Note

Actual workflow files, database credentials, API keys, and datasets are not included in this repository for security and privacy reasons. A sample dataset and workflow architecture image are provided.

# Outcome
This solution enables business users to retrieve information from a database without writing SQL queries, reducing dependency on technical teams and making data access faster and more user-friendly.



