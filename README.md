# AI-Powered Chatbot for Supplier and Product Information

**Revolutionizing Supplier and Product Data Queries Using AI **

---

## Overview

This project delivers an **AI-Powered Chatbot** designed to simplify querying supplier and product information using natural language. By leveraging open-source **Large Language Models (LLMs)** and the **LangGraph framework**, the chatbot enables users to retrieve and summarize data from a structured database. This application bridges the gap between complex data systems and user-friendly interaction, enhancing operational efficiency and decision-making.

---

## Key Features

- **Natural Language Querying**: Interact using simple text inputs to fetch supplier and product data.
- **LLM Integration**: Summarizes supplier information and provides context-driven responses.
- **Database Integration**: Efficiently fetch product and supplier information using MySQL/PostgreSQL.
- **Conversation History**: Displays recent queries and responses for seamless interaction.
- **Scalable Architecture**: Suitable for small to large-scale implementations.
- **Error Handling**: Manages missing or incorrect queries gracefully.

---

## Technologies Used

### **Backend**
- **Python** (Flask/FastAPI)
- **LangGraph Framework**
- **Open-Source LLMs** (Hugging Face GPT-2, GPT-3, LLaMA 2)

### **Frontend**
- **React** (with Material UI or Tailwind CSS)
- **Axios** (for API calls)
- **State Management** (Redux/Context API)

### **Database**
- **MySQL/PostgreSQL**

---

## Functional Workflow

### **Chatbot Workflow**

1. **User Query**:
   - Users input natural language queries like:
     - *"Show me all products under brand X."*
     - *"Which suppliers provide laptops?"*
     - *"Give me details of product ABC."*

2. **Data Retrieval**:
   - LangGraph nodes interact with the database to fetch relevant supplier or product information.

3. **LLM Summarization**:
   - Supplier data and contextual information are summarized using an open-source LLM.

4. **Response Generation**:
   - The chatbot returns structured, accurate, and context-enhanced responses.

---

## Installation

### **Prerequisites**

- Python 3.8+
- Node.js 14+
- MySQL/PostgreSQL
- pip
- git

---

### **Backend Setup**

1. Clone the repository:
   ```bash
   https://github.com/anurag8773/AI-Powered-Chatbot
   ```

2. Install backend dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Configure the database:
   - Update `config.py` with your database credentials.

4. Initialize the database:
   ```bash
   python manage.py db_init
   ```

5. Run the backend server:
   ```bash
   python app.py
   ```

---

### **Frontend Setup**

1. Navigate to the frontend directory:
   ```bash
   cd ../frontend
   ```

2. Install frontend dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```

---

## Database Schema

### **Products Table**
| Field       | Type        | Description                    |
|-------------|-------------|--------------------------------|
| ID          | Integer (PK)| Unique identifier for products |
| Name        | String      | Product name                  |
| Brand       | String      | Brand name                   |
| Price       | Decimal     | Product price                |
| Category    | String      | Product category             |
| Description | Text        | Product description          |
| Supplier ID | Integer (FK)| Linked supplier identifier    |

### **Suppliers Table**
| Field        | Type        | Description                      |
|--------------|-------------|----------------------------------|
| ID           | Integer (PK)| Unique identifier for suppliers  |
| Name         | String      | Supplier name                   |
| Contact Info | String      | Contact information             |
| Categories   | String      | Product categories offered      |

---

## Usage

1. Access the application via the frontend web interface.
2. Enter your query into the chatbot text input field.
3. View structured, AI-enhanced responses in the conversational format.

---

### Feel free to contribute!

We welcome feedback and contributions to enhance this project further. Fork the repository and submit your pull requests to suggest improvements.

---
