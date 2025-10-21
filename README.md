# Vertex AI StackOverflow Q&A Fine-Tuning

This notebook demonstrates how to use **Google Cloud Vertex AI** and **BigQuery Public Datasets** to prepare and fine-tune a text generation model on Stack Overflow Q&A data.

## Steps
1. Connect to BigQuery and load Stack Overflow data.
2. Extract Python-related questions and answers.
3. Format data for instruction-based fine-tuning.
4. Save as JSONL for model training on Vertex AI.

## Requirements
- Google Cloud SDK (`gcloud`)
- Vertex AI SDK
- BigQuery SDK
- Python 3.10+

## Example output
Each training line contains:
```json
{"input_text_instruct": "Please answer this StackOverflow question...", "output_text": "Answer content..."}
