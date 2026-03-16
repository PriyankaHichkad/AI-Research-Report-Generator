---
TITLE: AI-Research-Report-Generator
AUTHOR: Priyanka Rajeev Hichkad
---

# Automated Research Report Generator

## Overview
The **Automated Research Report Generator** is an AI-powered workflow that automatically gathers information on a given topic, summarizes key insights, and generates a structured research report. The system uses AI agents together with web search tools to collect relevant information and deliver the final report via email.

The workflow is built using :contentReference[oaicite:0]{index=0} and demonstrates how AI agents can interact with external tools to automate multi-step tasks such as research, summarization, and communication.

---

# Introduction
In many situations, researching a new topic requires going through multiple websites, reading articles, and manually compiling information. This process can be time-consuming and inefficient, especially when large amounts of information need to be analyzed.

This project was created to automate the research process using an AI-driven workflow. The system accepts a research topic as input, searches the internet for relevant resources, extracts important insights, and generates a structured research report.

By combining AI reasoning with workflow automation, this project simulates a digital research assistant capable of gathering and organizing information automatically.

---

# Key Features

- Automated research on any user-provided topic  
- Web search integration for real-time information retrieval  
- AI-generated structured research reports  
- Multi-agent workflow design for modular task handling  
- Automatic report delivery through email  
- Fully automated pipeline from input to report generation  

---

# Workflow Architecture

The system follows a multi-step workflow designed using :contentReference[oaicite:1]{index=1}.

### 1. User Input
The workflow begins with a user providing a **research topic** through the input message node.

Example input:
Applications of Artificial Intelligence in Healthcare

---

### 2. Main AI Agent
The **Main AI Agent** acts as the controller of the workflow. It interprets the user's request and decides when to call other tools or agents to gather information.

The reasoning capabilities of the agent are powered by a chat model accessed through :contentReference[oaicite:2]{index=2}.

---

### 3. Chat Model
AI-powered research assistant using a chat model to search the web, generate reports, and send results via email.

---

### 4. Web Search Tool
The research agent uses :contentReference[oaicite:3]{index=3} to perform automated web searches. The tool retrieves relevant articles and web resources related to the research topic.

---

### 5. Report Generation
After collecting the necessary information, the AI agent compiles the extracted insights into a structured research report containing:

- Title  
- Introduction  
- Key Insights  
- Current Applications  
- Future Outlook  
- Conclusion  

---

### 6. Email Delivery
The generated research report is automatically sent to the user using the **Send Email node** integrated into the workflow.

---

# Technologies Used

- :contentReference[oaicite:4]{index=4} – Workflow automation and orchestration  
- :contentReference[oaicite:5]{index=5} – Access to AI chat models  
- :contentReference[oaicite:6]{index=6} – Web search API for retrieving research content  
- Email integration – Automated report delivery  

---

# AI Agent Design

The project uses a **two-agent architecture** to manage the workflow efficiently.

### Main AI Agent
- Interprets the user's research request  
- Coordinates the workflow execution  
- Generates the final research report  

### Research AI Agent
- Performs web searches  
- Collects relevant information from multiple sources  
- Extracts key insights for report generation  

This modular structure improves scalability and allows the workflow to be expanded with additional tools in the future.

---

# Project Demonstration

A complete video demonstration of the workflow execution is available through the Google Drive link below.

🎥 **Video Demonstration:**  
https://drive.google.com/file/d/14u49_9pDViZAKX2AIbsEjt0A81hOOLIr/view?usp=
drive_link

The demonstration video includes:

- Explanation of the project goal  
- Overview of the workflow nodes in the canvas  
- Live execution of the workflow  
- Demonstration of the AI agent using its tools  
- Email delivery of the generated research report  

---

# Workflow File

This repository also contains the exported workflow configuration file from :contentReference[oaicite:7]{index=7}.

📂 **Workflow JSON File**

The `workflow.json` file included in this repository contains the complete configuration of the automation workflow. This file can be imported directly into n8n to reproduce the project.

Steps to use the workflow file:

1. Open your n8n workspace.
2. Import the provided JSON workflow file.
3. Configure the required API credentials (SerpAPI, email service, etc.).
4. Run the workflow using your desired research topic.

This allows other users to easily replicate the automated research assistant.

---

# Challenges Faced

### AI Agent Not Using Tools
Initially, the AI agent generated responses without using external tools. This issue was resolved by improving the tool descriptions and system prompts so that the agent explicitly called the search tool when performing research.

### API Authentication Issues
Configuring API credentials correctly was necessary for tools such as SerpAPI and the email service. After properly setting the credentials within the workflow platform, the tools were able to connect successfully.

### Email Formatting
The AI initially generated responses in Markdown format, which appeared incorrectly in emails. This issue was solved by instructing the agent to return the final report in plain text format.

---

# Future Improvements

Several improvements could enhance the functionality of this system:

- Integration with academic research databases  
- Adding webpage content extraction tools  
- Generating downloadable PDF reports  
- Storing research reports in cloud storage  
- Building a simple web interface for user interaction  

---

# Conclusion

This project demonstrates how AI agents can be integrated with workflow automation to create intelligent systems capable of performing complex tasks such as automated research and summarization.

By combining AI reasoning with web search and communication tools, the **Automated Research Report Generator** provides an efficient way to gather and summarize information with minimal human effort.

The project highlights the potential of AI-driven workflow automation in improving productivity and simplifying information-intensive tasks.

