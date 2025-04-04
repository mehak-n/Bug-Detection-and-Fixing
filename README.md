
🐍 Python Bug Detection and Fix Generation System
An AI-powered system that detects and fixes bugs in Python code snippets using a BERT-based classifier and a large language model. Designed to assist developers and learners in quickly identifying errors and generating fixes automatically.

🚀 Project Overview
Debugging is often time-consuming, especially for beginners. This project combines a Bug Detection Model and a Fix Generation API to provide a streamlined way of catching and correcting Python code errors. It uses a BERT classifier to detect buggy code and leverages Mistral-7B-Instruct (via HuggingFace API) to suggest fixes.

📌 Key Features
⚙️ Bug Detection Model using BERT

🔧 Automatic Fix Generation with LLM

📊 Evaluation Reports with BLEU & similarity metrics

🧠 Educational tool to teach Python debugging

📈 High accuracy in identifying buggy code

🧠 Model Architecture
🔍 Bug Detection
Model: bert-base-uncased

Classifier: Linear layer on pooled BERT output

Task: Binary classification (Buggy / Bug-Free)

🛠️ Fix Generation
Model: Mistral-7B-Instruct via HuggingFace API

Input: Buggy Python code + task prompt

Output: Corrected Python code

📂 Dataset
✅ 100+ Python code snippets

🐞 Binary labels: 1 for buggy, 0 for bug-free

🔧 Fixes included for buggy samples

⚙️ Tokenized using Python’s tokenize module + BERT tokenizer

🔁 Workflow
Input a Python code snippet

Run Bug Detection Model to classify it

If buggy, send to Fix Generator API

Return classification and suggested fix

📊 Results & Performance
🧪 Bug Detection Metrics
Accuracy: 91.30%

Precision: 91.30%

Recall: 100.00%

F1-Score: 95.45%

📌 Discussion: Excellent at catching bugs, slightly weak on identifying bug-free code due to class imbalance.

🧪 Fix Generation Metrics
Average Similarity Score: 15.26%

Average BLEU Score: 11.70%

Median Similarity Score: 20.22%

Median BLEU Score: 14.72%

📌 Discussion: Fixes are syntactically correct but may diverge from ground truth. Prompt refinement and model fine-tuning are needed.

🔮 Future Improvements
Fine-tune BERT on code-focused datasets

Replace Mistral with CodeLlama or StarCoder

VS Code extension for real-time debugging

Add explanation generator for fixes
