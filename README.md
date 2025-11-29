<img width="1905" height="964" alt="image" src="https://github.com/user-attachments/assets/819a4c38-d841-4a5b-af80-70868d850b02" />📚 Smart Study Mentor – Multi-Agent Learning Assistant (SSM-A)
Personalized learning powered by multi-agent AI — Diagnose Weaknesses · Generate Micro-Lessons · Track Progress Over Time

🚀 Overview
Smart Study Mentor (SSM-A) is a multi-agent learning assistant built using Google’s Agent Development Kit (ADK).
Instead of acting like a static chatbot, it behaves like a small team of teaching assistants, each specializing in a different part of the learning pipeline:
📌 Student Intake Agent – understands subjects, topics, and study goals
🧠 Weakness Detector Agent – generates quizzes & evaluates performance
✍️ Lesson Generator Agent – creates micro-explanations & practice sets
📈 Progress Tracker Agent – stores learning history using long-term memory
The system forms a feedback loop:
Assess → Teach → Practice → Remember → Improve
SSM-A was developed as part of the Kaggle × Google AI Agents Intensive (2025) Capstone Project.

🎯 Problem Statement
Engineering and AI/DS students often struggle with:
Deciding what to study
Identifying weak areas
Finding crisp explanations
Tracking improvement across sessions
Self-study becomes inefficient—students spend more time planning than learning.

🤖 Why Agents?
A single chatbot cannot diagnose weaknesses, generate specialized content, search information, and track student progress at the same time.
A multi-agent system solves this by distributing roles:
Each agent has a specific responsibility
The orchestrator coordinates them in a sequence
Tools and memory enable personalized, context-aware study sessions
Agents allow SSM-A to behave more like a team of tutors rather than a single assistant.

🏗️ Architecture

Study Session Manager
      ▼
Intake Agent
(goals/topics)
      ▼
Weakness Agent
(quiz + eval)
      ▼
Lesson Generator
(micro-lessons) 
      ▼
Progress Tracker
(Memory)

🔑 Key Components
Multi-agent pipeline (sequential)
Custom Python Tools
Quiz generator
Quiz evaluator
MCP / Google Search Tool Integration
Session Memory for single-session context
Long-term Memory Bank for progressive learning
Observability: Logs, traces, metrics

🧪 Demo
A typical study session:
Student selects subject & topics
Weakness Detector agent runs a quiz
Weak topics identified
Lesson Generator produces concise micro-lessons
Progress Tracker saves:
quiz score
weak topics
next study recommendation
On the next session, SSM-A adapts based on stored history

🔧 Technologies Used
Google ADK (Python)
Gemini Model (LLM)
Custom Tools (Quiz generator & evaluator)
Memory Bank for long-term adaptation
MCP / Search Tools for external knowledge
Kaggle Notebook for development and execution

📈 Value
SSM-A helps students:
study smarter with targeted micro-lessons
improve faster through weakness-based learning
track progress with long-term memory
save time by eliminating manual planning
This is especially powerful for fast-paced courses like AI, ML, Data Science, and Engineering.

🛠️ If I Had More Time
Future enhancements include:
Adding spaced repetition (SRS)
Multi-language support
Support for uploading textbooks/syllabus PDFs
Dashboard for progress visualization
Deployment to Vertex AI Agent Engine
Adaptive difficulty levels for quizzes

📄 License
This project is licensed under the MIT License — free to use, modify, and share with attribution.

🙌 Acknowledgements
Google’s Agent Development Kit (ADK)
Kaggle Agents Intensive Course Team
Gemini Model for LLM reasoning
