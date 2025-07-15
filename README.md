# 🔥  Natural Language to SQL Generation using Open-Source LLMs

A two-stage generative AI system that converts natural language questions into SQL queries, using schema-linking and fine-tuned Large Language Models (LLMs). Built during my final-year project at AxeFinance.

## 🚀 Features
- Two-stage architecture:
  - **Schema Linking Model**: Identifies correct tables & columns.
  - **SQL Generation Model**: Generates SQL queries.
- Fine-tuned open-source models (Mistral, LLaMA).
- API endpoint built using FastAPI.
- Dataset: [Spider benchmark](https://yale-lily.github.io/spider).
- Achieved **83.46% execution accuracy** on Spider.

## 📷 Demo
![demo](screenshots/demo.gif)

## 📦 Technologies Used
- Python
- Hugging Face Transformers
- PEFT / LoRA
- PyTorch
- FastAPI
- SQL Server (for testing)
- Google Colab (for training)

## 📊 Results
- Execution Accuracy: 83.46%
- Schema Linking Accuracy: 91.66%
- Ranked 3rd on Spider Benchmark 

## 🔗 Models on Hugging Face

- [Schema-Linking Model](https://huggingface.co/houssemmoslah/mistral_schema_linking1_merged)
- [SQL Generation Model](https://huggingface.co/houssemmoslah/mistral_sql_gen6000_merged-GGUF)



## 🚀 How to Run
```bash
pip install -r requirements.txt
uvicorn src.api:app --reload

