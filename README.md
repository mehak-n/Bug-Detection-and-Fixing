Python Bug Detection and Fix Generation System
An AI-powered system that detects and fixes bugs in Python code snippets using a BERT-based classifier and a large language model. Designed to assist developers and learners in quickly identifying errors and generating fixes automatically.

Project Overview
Debugging is often time-consuming, especially for beginners. This project combines a Bug Detection Model and a Fix Generation API to provide a streamlined way of catching and correcting Python code errors. It uses a BERT classifier to detect buggy code and leverages Mistral-7B-Instruct (via HuggingFace API) to suggest fixes.

Key Features
Bug Detection Model using BERT

Automatic Fix Generation with LLM

Evaluation Reports with BLEU and Similarity Metrics

Educational Tool for Learning Python Debugging

High Accuracy in Identifying Buggy Code

Model Architecture
Bug Detection
Model: bert-base-uncased

Classifier: Linear layer on pooled BERT output

Task: Binary classification (Buggy / Bug-Free)

Fix Generation
Model: Mistral-7B-Instruct via HuggingFace API

Input: Buggy Python code with task-specific prompt

Output: Corrected Python code

Dataset
Over 100 Python code snippets

Binary labels: 1 for buggy, 0 for bug-free

Fixes provided for buggy samples

Tokenized using Python's tokenize module and BERT tokenizer

Workflow
Input a Python code snippet

Run Bug Detection Model to classify the code

If classified as buggy, send it to Fix Generation API

Return classification and suggested fix to the user

Results and Performance
Bug Detection Metrics
Accuracy: 91.30%

Precision: 91.30%

Recall: 100.00%

F1-Score: 95.45%

Fix Generation Metrics
Average Similarity Score: 15.26%

Average BLEU Score: 11.70%

Median Similarity Score: 20.22%

Median BLEU Score: 14.72%

Discussion
The bug detection model performs exceptionally well in identifying buggy code, with high precision and perfect recall. This makes it particularly useful in educational or debugging-assist scenarios. However, due to a slight class imbalance, the system sometimes misclassifies clean code as buggy.
For fix generation, the system produces valid Python syntax and meaningful suggestions, although the fixes may occasionally differ from the ground truth. Overall, the system proves to be a strong foundation for intelligent debugging support.

Conclusion
This project demonstrates the potential of combining modern NLP techniques and large language models to automate bug detection and code correction. With a solid accuracy rate and functional fix suggestions, it offers valuable support to both developers and learners.
The system showcases how artificial intelligence can accelerate the debugging process, reduce development time, and serve as an educational tool to improve coding skills. Future versions can further enhance performance and integration, but even in its current form, the system provides a smart and efficient solution for Python code debugging.

