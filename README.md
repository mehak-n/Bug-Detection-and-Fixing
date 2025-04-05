Python Bug Detection and Fix Generation System

An AI-powered tool that detects and fixes bugs in Python code using a BERT-based classifier and Mistral-7B-Instruct via HuggingFace API. It helps developers and learners quickly identify errors and generate fixes.

Key Features:

Bug detection using bert-base-uncased

Fix generation via large language model

Evaluation using BLEU and similarity scores

Supports learning and fast debugging

Workflow:

Input a Python code snippet

BERT model classifies as buggy or clean

If buggy, LLM suggests a corrected version

Returns classification and fix

Performance:

Detection accuracy: 91.3%, F1-Score: 95.45%

Fix quality (BLEU): Avg. 11.70%, Median: 14.72%

Conclusion: Combining NLP with LLMs, the system offers an efficient way to debug Python code and assist in coding education.
