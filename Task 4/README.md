# Task 4: General Health Query Chatbot (Prompt Engineering Based)

## 🔍 Task Objective
The goal of this task is to develop a simple and safe chatbot capable of answering general health-related questions using a Large Language Model (LLM). The chatbot leverages prompt engineering to ensure responses are friendly, informative, and cautious, with built-in safeguards to avoid harmful medical advice.

## 📦 Dataset Used
No external dataset was required for this task. The chatbot uses the pretrained knowledge embedded within the Mistral-7B-Instruct model, accessed via the Hugging Face API.

## 🤖 Model Applied
- **Model:** [Mistral-7B-Instruct](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.1)
- **Source:** Hugging Face Inference API
- **Access Method:** `transformers` and `huggingface_hub` libraries in Python
- **Prompt Engineering:**
  - System prompts are designed like:  
    _"You are a helpful and friendly medical assistant. Answer general health-related questions clearly and cautiously. Avoid giving direct medical advice or dosage recommendations."_

## 🧪 Key Features and Safety Measures
- Accepts user input through a command-line interface or notebook cell
- Embeds clear disclaimers to ensure the chatbot doesn't replace a medical professional
- Rejects or deflects unsafe, harmful, or ethically sensitive queries
- Avoids giving explicit prescriptions, treatments, or critical diagnosis

## 💬 Sample Queries and Behavior
- **Input:** What causes a sore throat?  
  **Response:** Explains common causes like viral infections, environmental irritants, etc., with a disclaimer to consult a doctor for persistent symptoms.

- **Input:** Is paracetamol safe for children?  
  **Response:** Mentions general safety in proper doses but avoids giving dosage; recommends consulting a pediatrician.

## ✅ Key Results and Findings
- **Mistral-7B-Instruct** performed well for short, general queries, maintaining tone and clarity with engineered prompts.
- Prompt structure significantly influenced safety and helpfulness.
- Hugging Face API made it easy to test open-source LLMs without GPU setup.

## 📌 Conclusion
This task illustrates how open-source models like Mistral-7B-Instruct can power helpful health chatbots when combined with thoughtful prompt engineering and ethical safety constraints. It reinforces that while LLMs are useful for general education, they should never replace real medical consultation.

---


