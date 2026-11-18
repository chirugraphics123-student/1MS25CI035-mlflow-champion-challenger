# Champion–Challenger Model Comparison: Sentiment Classification

**Student USN:** `1MS25CI035`  
**Course:** Skill Lab (MLOps with MLflow)

---

## 1. Task and Models
* **Task:** Binary Sentiment Classification (`sentiment-analysis`)
* **Dataset:** GLUE `nyu-mll/glue` (`sst2` validation split), fixed random subset of **200 samples** (`seed = 42`), saved to `data/eval_inputs.csv`.
* **Model A (Current Champion):** `distilbert-base-uncased-finetuned-sst-2-english` (~67M parameters, fast baseline)
* **Model B (Challenger Candidate):** `siebert/sentiment-roberta-large-english` (~355M parameters, larger RoBERTa architecture)

---

## 2. How to Run
Run these commands in order from the project root directory on Windows PowerShell:

1. **Create and activate virtual environment, then install dependencies:**
   ```powershell
   py -m venv .venv
   .\.venv\Scripts\Activate.ps1
   pip install -r requirements.txt