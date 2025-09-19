# 🔧 Fine-Tuning Google T5-Small on SQL-Create-Context

This project fine-tunes **Google’s T5-Small** model on the [SQL-Create-Context dataset](https://huggingface.co/datasets/b-mc2/sql-create-context) to answer natural language questions with SQL/table context.  
It demonstrates how to adapt pretrained language models for **domain-specific tasks**.

---

## 📌 Features
- End-to-end **fine-tuning workflow** with Hugging Face `transformers`
- Input formatting: question: <QUESTION> context: <CONTEXT>
- Training using `Seq2SeqTrainer` with periodic evaluation
- **BLEU-1 to BLEU-4** metrics for detailed evaluation
- Training/validation loss visualization
- Simple inference demo

---

## 📊 Results

| Step | Train Loss | Val Loss | BLEU  | BLEU-1 | BLEU-2 | BLEU-3 | BLEU-4 |
|------|------------|----------|-------|--------|--------|--------|--------|
| 500  | 0.3807     | 0.2516   | 71.68 | 87.17  | 76.56  | 71.85  | 67.50 |
| 1000 | 0.2150     | 0.1628   | 78.18 | 90.40  | 81.95  | 78.10  | 74.56 |
| 1500 | 0.1951     | 0.1424   | 80.79 | 92.02  | 84.83  | 81.26  | 77.98 |

---
