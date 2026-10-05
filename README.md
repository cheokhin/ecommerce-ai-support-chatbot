# E-Commerce AI Support Chatbot ("Sonny")

**🔴 Live Demo:** [Click here to chat with the AI](insert-your-surviving-replit-link-here)

*Note: The original backend source code was lost during a cloud environment deprecation on Replit. This repository serves to showcase the functioning live deployment, system architecture, and technical methodologies used to build the pipeline.*

## Project Objective
Developed "Sonny," an intelligent AI customer support chatbot for a fictional e-commerce platform (Sunshine Tech). The bot automates routine customer service tasks, drastically reducing wait times by handling order tracking, product inquiries, and support ticket generation through structured workflows and AI classification.

## Tech Stack & Core Methodologies
* **Platforms & Tools:** Botpress, Replit (Deployment)
* **Languages:** JavaScript (utilized within Botpress 'Execute Code' cards)
* **Databases:** Table Database (for structured data like shipping statuses and user records)
* **Methodologies:** Text Similarity Algorithms, Retrieval-Augmented Generation (RAG), Modular Workflow Design
* **LLM Integration:** [Insert the specific LLM you used, e.g., OpenAI GPT-3.5 API / Llama / Gemini]

## System Architecture & Logic

### 1. Intelligent Routing & Core Workflows
Engineered a user-centered, modular architecture that forces AI classification on user inputs, routing them efficiently through 5 distinct workflows:
* **Track Order:** Validates user order IDs and retrieves real-time shipping statuses directly from the database.
* **Store Info:** Provides operational details and intelligent store navigation.
* **Product Inquiry:** Utilizes a text similarity algorithm to calculate matching percentages and retrieve the most relevant product descriptions.
* **QnA (Knowledge Base):** Searches the internal knowledge base to formulate accurate answers for general queries.
* **Support Ticket:** Automatically gathers user information (name, email, order ID, issue description) and writes structured data to the database to escalate complex issues to human agents.

### 2. Knowledge Retrieval (RAG Pipeline)
* Embedded short product descriptions and FAQs into the knowledge base to be dynamically queried.
* Applied text similarity algorithms to ensure the bot fetches the most relevant and accurate information based on the user's natural language input, effectively preventing AI hallucinations.

### 3. Data Management & User Experience
* Managed structured data operations using JavaScript, executing backend logic to read records (like valid order IDs) and write new data (like support tickets).
* Implemented an automated feedback loop, prompting users to rate their experience before ending the conversation to gather analytical metrics.
