# TOPSIS-Based Pre-trained Model Selection for Text Classification  
Roll Number: 102353017

## Overview
This project applies the TOPSIS (Technique for Order Preference by Similarity to Ideal Solution) method to select the best pre-trained model for a text classification task. Instead of relying on a single metric, multiple performance and efficiency criteria are considered to make a balanced decision.

All datasets and models are taken from Hugging Face.

---

## Dataset
The IMDB movie reviews dataset from Hugging Face is used.  
To avoid class imbalance, a balanced subset is created consisting of:
- 150 positive reviews  
- 150 negative reviews  

This ensures fair comparison across models.

---

## Models Used
The following pre-trained transformer models from Hugging Face are evaluated:
- BERT (bert-base-uncased)
- DistilBERT (distilbert-base-uncased)
- RoBERTa (roberta-base)
- MobileBERT (google/mobilebert-uncased)

The models are evaluated in a pre-trained (zero-shot) setting without task-specific fine-tuning.

---

## Evaluation Criteria
Each model is evaluated using the following parameters:
- Accuracy (benefit criterion)
- Inference Time in milliseconds (cost criterion)
- Model Size in MB (cost criterion)

F1-score is not used in TOPSIS since the models are not fine-tuned and F1 can be unstable in such settings.

---

## Methodology
1. Load dataset and models from Hugging Face  
2. Perform inference on the balanced dataset  
3. Record accuracy, inference time, and model size  
4. Construct the decision matrix  
5. Normalize and weight the criteria  
6. Apply the TOPSIS method  
7. Rank the models based on TOPSIS score  

---

## Results
The TOPSIS results show that **MobileBERT** achieves the highest overall score due to its good balance of accuracy, fast inference time, and small model size.

Screenshots included in the repository:
<img width="891" height="101" alt="image" src="https://github.com/user-attachments/assets/635c45fd-e48e-4e28-97c8-b8395f5fc7be" />

<img width="557" height="471" alt="image" src="https://github.com/user-attachments/assets/98dca82a-e19e-47d0-8c3f-4b3385c50e23" />

- `topsis_score_table.png`
- `topsis_score_graph.png`

---

## Tools and Libraries
- Python
- Google Colab
- Hugging Face (Transformers and Datasets)
- Scikit-learn
- Pandas
- NumPy
- Matplotlib

---

## Conclusion
This project demonstrates that selecting models using multiple criteria provides a more practical evaluation than using accuracy alone. TOPSIS helps identify a model that balances performance and efficiency, making it suitable for real-world applications.

---

## Repository Structure
- TOPSIS_Text_Classification_102353017.ipynb  
- README.md  





