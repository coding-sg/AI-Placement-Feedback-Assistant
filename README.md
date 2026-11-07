# AI Placement Feedback Assistant

An AI-powered platform designed to help students prepare for technical placement interviews through simulated interview questions, automated answer evaluation, performance scoring, and personalised improvement suggestions.

Built using **Streamlit, LangChain, LangGraph, and Google Gemini**, this project demonstrates how Large Language Models (LLMs) can be integrated into a structured AI workflow to support interview preparation.

## Project Overview

Preparing for technical interviews requires more than just knowing the subject. Candidates also need to communicate their knowledge clearly, provide relevant answers, and identify areas where they need improvement.

The AI Placement Feedback Assistant addresses this by allowing users to practise interview questions and receive AI-generated evaluations of their responses.

The application analyses each answer, assigns a score out of 10, and provides additional feedback when the performance score is below the defined threshold.

## Key Features

- **Role-Based Interview Questions:** Generate interview questions based on the selected job role.
- **Custom Questions:** Practise using questions entered by the user.
- **AI-Based Answer Analysis:** Evaluate responses based on technical correctness, relevance, clarity, and completeness.
- **Performance Scoring:** Receive a score out of 10 using a predefined evaluation rubric.
- **Personalised Feedback:** Get suggestions and sample improved answers for responses scoring below 7.
- **Evaluation Report:** Generate a final interview assessment report.
- **Report Download:** Download the generated evaluation report for future reference.

## How It Works

The application follows a multi-step workflow implemented using LangGraph.

1. **Question Selection:** The user selects a job role and generates a question or enters a custom question.
2. **Answer Submission:** The user provides an answer to the interview question.
3. **Answer Analysis:** Gemini analyses the response based on predefined evaluation criteria.
4. **Performance Evaluation:** The system assigns a score between 0 and 10.
5. **Conditional Feedback:** If the score is below 7, the workflow generates detailed improvement suggestions and a sample answer.
6. **Final Report:** The system generates a consolidated evaluation report.

## Technology Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Streamlit | Interactive web application |
| Google Gemini API | LLM-based question generation and evaluation |
| LangChain | LLM integration and prompt execution |
| LangGraph | Workflow orchestration and conditional routing |
| LangSmith | LLM application monitoring |
| Pydantic | Data validation |
| Python-dotenv | Environment variable management |

**LLM Model:** Gemini 3.5 Flash

## Project Structure

```text
AI-Placement-Feedback-Assistant/
│
├── app.py
├── graph.py
├── nodes.py
├── state.py
├── requirements.txt
├── .env
└── README.md
```

| File | Description |
|---|---|
| `app.py` | Streamlit user interface |
| `graph.py` | Defines and compiles the LangGraph workflow |
| `nodes.py` | Contains LLM-powered question generation, analysis, evaluation, feedback, and reporting functions |
| `state.py` | Defines the state structure shared across workflow nodes |
| `requirements.txt` | Lists project dependencies |
| `.env` | Stores local environment variables |

## Installation and Setup

### 1. Clone the Repository

### 2. Create a Virtual Environment

### 3. Install Dependencies

### 4. Configure Gemini API Key

Create a `.env` file in the project directory:

### 5. Run the Application

```bash
streamlit run app.py
```

## Learning Outcomes

Through this project, I gained practical experience in:

- Integrating Google Gemini with LangChain.
- Building multi-step AI workflows using LangGraph.
- Implementing conditional routing based on model-generated evaluation scores.
- Designing prompts for answer analysis and evaluation.
- Developing interactive applications using Streamlit.
- Managing LLM application workflows and monitoring.

## Acknowledgement

I would like to express my gratitude to **Innomatics Research Labs** for providing the learning opportunity, technical guidance, and practical exposure that helped me explore Generative AI, LangChain, LangGraph, and LLM-powered application development.
