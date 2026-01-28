# TOPSIS for Pre-trained Text Summarization Models

This project applies the **TOPSIS (Technique for Order Preference by Similarity to Ideal Solution)** method to select the best pre-trained model for **Text Summarization**.

## Models Evaluated
- BART Large
- T5 Base
- PEGASUS
- DistilBART

## Evaluation Criteria
| Criteria | Type |
|--------|------|
| ROUGE Score | Benefit (+) |
| Inference Time | Cost (-) |
| Model Size | Cost (-) |
| Memory Usage | Cost (-) |

## Steps
1. Normalize decision matrix
2. Apply weights
3. Identify ideal best and worst
4. Compute distances
5. Rank models using TOPSIS score

## How to Run
```bash
pip install -r requirements.txt
cd src
python summarization_models.py
