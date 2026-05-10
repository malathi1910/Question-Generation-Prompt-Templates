<div align="center"> <h1>🎯 Controlled Question Generation Using Prompt Templates</h1> <h3>AI-powered Prompt Engineering System for Intelligent Question Generation</h3> <img src="https://img.shields.io/badge/Prompt%20Engineering-AI-blue?style=for-the-badge" /> <img src="https://img.shields.io/badge/Domain-Specific-success?style=for-the-badge" /> <img src="https://img.shields.io/badge/Difficulty-Control-important?style=for-the-badge" /> <img src="https://img.shields.io/badge/JSON-Structured-orange?style=for-the-badge" /> </div>
📌 Project Overview

This project focuses on designing structured prompt templates for controlled AI-based question generation.

The system generates:

✅ Domain-specific questions
✅ Difficulty-controlled questions
✅ Context-aware follow-up questions
✅ Non-repetitive and structured outputs

The prompts are designed for applications such as:

🎓 Educational Platforms
💼 AI Interview Systems
📝 Online Assessment Tools
📚 Adaptive Learning Systems
🎯 Objective

The main objective of this project is to create reusable prompt templates that guide AI models to generate:

High-quality questions
Difficulty-specific questions
Context-aware follow-up questions
Diverse and non-repetitive topics

The system also ensures:

Domain relevance
Difficulty consistency
Structured JSON responses
Topic variation
🚀 Features
Feature	Description
✅ Domain-Specific Generation	Questions belong strictly to the provided domain
✅ Difficulty Control	Supports Easy, Medium, and Hard levels
✅ Context Awareness	Generates intelligent follow-up questions
✅ Topic Variation	Prevents repetition and ensures diversity
✅ Structured Output	Returns responses in JSON format
✅ Edge Case Handling	Handles invalid or missing inputs
🛠️ Technologies Used
Technology	Purpose
🤖 Prompt Engineering	AI Prompt Design
🧠 Generative AI Concepts	Intelligent Question Generation
📄 JSON Formatting	Structured Outputs
🔤 NLP Concepts	Language Understanding
📂 Prompt Templates Included
1️⃣ Base Question Prompt
📌 Purpose

Generates a standard domain-specific question based on difficulty level.

🧾 Prompt Template
You are an expert question generator.

Generate ONE high-quality question based on the following input:
- Domain: {domain}
- Difficulty: {difficulty}

Rules:
- The question must strictly belong to the given domain.
- Difficulty must match:
  - easy → basic concept/definition
  - medium → application-based
  - hard → problem-solving or analytical
- Avoid vague or generic questions.
- Do NOT repeat previously generated questions.
- If domain is missing, use "General Computer Science".
- If difficulty is invalid, default to "medium".

Output format (JSON only):
{
  "question": "...",
  "topic": "...",
  "difficulty": "..."
}
📥 Example Input
{
  "domain": "DSA",
  "difficulty": "medium"
}
📤 Example Output
{
  "question": "Explain how binary search works on a sorted array and analyze its time complexity.",
  "topic": "Searching Algorithms",
  "difficulty": "medium"
}
2️⃣ Context-Aware Prompt
📌 Purpose

Generates intelligent follow-up questions using:

Previous question
Candidate answer
Difficulty level
🧾 Prompt Template
You are an intelligent interviewer.

Generate a follow-up question based on:
- Domain: {domain}
- Previous Question: {previous_question}
- Candidate Answer: {candidate_answer}
- Difficulty: {difficulty}

Rules:
- The question must be relevant to the domain.
- It should build on the previous question.
- If the answer is correct → ask a deeper or advanced question.
- If the answer is weak/incorrect → ask a clarifying or foundational question.
- Maintain the specified difficulty level.
- Avoid repeating the same question or topic.

Output format (JSON only):
{
  "question": "...",
  "topic": "...",
  "difficulty": "..."
}
3️⃣ Difficulty-Control Prompt
📌 Purpose

Strictly enforces question difficulty levels.

🧾 Prompt Template
You are a strict difficulty-controlled question generator.

Generate ONE question based on:
- Domain: {domain}
- Difficulty: {difficulty}

Strict Rules:
- easy → only definitions, basic concepts, or simple explanations
- medium → application-based or example-driven questions
- hard → complex problem-solving, coding, or analytical reasoning

Additional Constraints:
- Do NOT mix difficulty levels.
- Do NOT generate vague or general questions.
- Ensure the question is domain-specific.
- If difficulty is invalid, default to "medium".
4️⃣ Topic Variation Prompt
📌 Purpose

Ensures topic diversity and prevents repetition.

🧾 Prompt Template
You are a question generator that ensures topic diversity.

Generate ONE question based on:
- Domain: {domain}
- Difficulty: {difficulty}
- Previously Covered Topics: {topics_list}

Rules:
- The question must belong to the given domain.
- Do NOT repeat any topic from the previously covered topics.
- Select a different subtopic within the domain.
- Maintain the required difficulty level.
- Avoid vague or generic questions.
⚙️ Constraints Handled

The system prevents:

❌ Repeated questions
❌ Vague questions
❌ Out-of-domain content
🧩 Edge Cases Handling
Edge Case	Handling Method
Missing Domain	Defaults to "General Computer Science"
Invalid Difficulty	Defaults to "medium"
Repeated Topics	Uses topic variation logic
Weak Candidate Answer	Generates foundational follow-up questions
✅ Acceptance Criteria
Requirement	Status
Domain Accuracy	✅ Achieved
Difficulty Consistency	✅ Achieved
Structured Output	✅ Achieved
Topic Diversity	✅ Achieved
Non-Repetitive Generation	✅ Achieved
🚀 Future Enhancements
🌐 Flask/FastAPI Integration
🗄️ Database Connectivity
🤖 AI-Based Answer Evaluation
📊 Adaptive Interview Systems
💻 Automatic Coding Question Generation
📖 Conclusion

This project demonstrates how prompt engineering can be used to build a controlled AI-based question generation system.

The designed prompts ensure:

Consistency
Domain relevance
Difficulty control
Structured outputs
Topic diversity
<div align="center">
</div>
