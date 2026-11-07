## AI Placement Feedback Assistant

An AI-powered interview preparation application built using **Python, Streamlit, LangChain, LangGraph, and Google Gemini**.

The application helps students prepare for technical interviews by generating role-specific questions, analysing submitted answers, evaluating performance, and providing personalised improvement feedback.

## Features

- **AI Interview Question Generation:** Generates technical interview questions based on the selected job role.
- **Custom Questions:** Allows users to enter their own interview questions.
- **Answer Analysis:** Analyses answers based on technical correctness, relevance, clarity, and completeness.
- **Performance Evaluation:** Assigns a score out of 10 using a defined evaluation rubric.
- **Personalised Feedback:** Provides suggestions for improving answers.
- **Sample Improved Answers:** Generates example answers to help students understand how to improve.
- **Evaluation Dashboard:** Displays the latest evaluation results.
- **Downloadable Reports:** Allows users to download their interview evaluation reports.
- **Conditional Workflow:** Uses LangGraph to determine whether additional feedback is required based on the evaluation score.

## Technology Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Streamlit | Interactive web application interface |
| LangChain | Integration with the language model |
| LangGraph | Workflow orchestration and conditional routing |
| Google Gemini API | AI-powered question generation and answer evaluation |
| LangSmith | Workflow monitoring and tracing |
| Pydantic | Data validation and structured data handling |

**AI Model:** Google Gemini (configured model: `gemini-3.5-flash`)

## Application Workflow

The application follows a multi-step AI workflow:

1. **Generate Interview Question:** Generates a technical interview question based on the selected job role.
2. **Analyse Answer:** Analyses the student's submitted answer.
3. **Evaluate Answer:** Assigns a score based on the following rubric:
   - Technical correctness: 0–4 marks
   - Relevance: 0–2 marks
   - Clarity: 0–2 marks
   - Completeness: 0–2 marks
4. **Conditional Routing:**
   - Score below 7: Proceeds to the feedback generation node.
   - Score 7 or above: Proceeds directly to report generation.
5. **Generate Final Report:** Creates a report containing the job role, interview question, evaluation score, answer analysis, improvement feedback, and final recommendation.

### File Description

- `app.py` – Streamlit user interface.
- `nodes.py` – Gemini integration and AI workflow functions.
- `graph.py` – LangGraph workflow definition and conditional routing.
- `state.py` – Defines the interview workflow state.
- `requirements.txt` – Project dependencies.
- `.gitignore` – Specifies files excluded from Git tracking.

## Installation and Execution

### 1. Clone the repository

### 2. Create a virtual environment

### 3. Install dependencies

### 4. Configure the Gemini API key

Create a `.env` file in the project directory:

### 5. Run the application

```bash
streamlit run app.py
```

## Learning Outcomes

This project provided practical experience in:

- Working with Large Language Models (LLMs).
- Integrating Google Gemini using LangChain.
- Building multi-step AI workflows using LangGraph.
- Implementing conditional routing in AI applications.
- Designing prompt-based answer evaluation systems.
- Developing interactive applications using Streamlit.
- Exploring AI workflow monitoring using LangSmith.

## Acknowledgements

I would like to express my sincere gratitude to **Innomatics Research Labs** for providing the training, practical learning opportunities, and guidance that helped me explore Generative AI and develop this project.

Special thanks to the trainers and mentors for introducing us to technologies such as LangChain, LangGraph, and LLM integration, and for encouraging us to apply these concepts through hands-on projects.