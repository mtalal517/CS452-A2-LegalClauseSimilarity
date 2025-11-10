Legal Clause Similarity — Baseline experiments

Contents
- `main.ipynb`: Jupyter notebook implementing data loading, pair generation, two siamese baselines (BiLSTM and BiLSTM+Attention), training loops, and evaluation metrics (Accuracy, F1, ROC-AUC).
- `requirements.txt`: minimal dependencies.

Quick start (PowerShell):

```powershell
python -m pip install -r requirements.txt
jupyter notebook
# open main.ipynb and run cells
```

Notes
- This project intentionally avoids using pre-trained transformer models per assignment constraints.
- Positive pairs are sampled from the same CSV category; negatives are sampled across categories — you can improve sampling strategy for better performance.

Next steps
- Run experiments with more epochs and tuned hyperparameters.
- Add subword tokenizer or pretrained embeddings (if allowed) to improve semantic capture.
- Implement cross-validation and logging of results (CSV) for comparison.
