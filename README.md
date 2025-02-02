# Assignment03---Topsis-for-Pretrained-Models
TEXT CLASSIFICATION
**Title: Evaluating Pre-Trained Models for Text Classification Using TOPSIS**

**1. Introduction**
Selecting the best pre-trained model for text classification requires balancing accuracy, inference time, and model size. This report applies the TOPSIS (Technique for Order of Preference by Similarity to Ideal Solution) method to rank popular models.

**2. Decision Criteria and Models Evaluated**
We considered four key criteria:

- **Accuracy (Higher is better)**
- **F1-score (Higher is better)**
- **Inference Time (Lower is better)**
- **Model Size (Lower is better)**

The following pre-trained models were evaluated:

- BERT
- RoBERTa
- DistilBERT
- XLNet
- ALBERT

**3. Data Collection and Normalization**
The following table presents the performance data:

| Model      | Accuracy | F1-score | Inference Time (ms) | Model Size (MB) |
| ---------- | -------- | -------- | ------------------- | --------------- |
| BERT       | 0.91     | 0.90     | 120                 | 420             |
| RoBERTa    | 0.92     | 0.91     | 130                 | 500             |
| DistilBERT | 0.89     | 0.88     | 80                  | 250             |
| XLNet      | 0.90     | 0.89     | 150                 | 450             |
| ALBERT     | 0.90     | 0.89     | 100                 | 300             |

Normalization was applied, and the TOPSIS method computed the Ideal Best and Ideal Worst values to derive rankings.

**4. Results and Rankings**
The final ranking based on TOPSIS scores is:

| Rank | Model      | TOPSIS Score |
| ---- | ---------- | ------------ |
| 1    | RoBERTa   | 0.8677       |
| 2    | BERT      | 0.6449       |
| 3    | XLNet     | 0.5861       |
| 4    | ALBERT    | 0.2911       |
| 5    | DistilBERT| 0.0000       |

A bar chart visualizing the rankings is included in the analysis.

**5. Conclusion**
RoBERTa emerged as the best choice due to its superior accuracy and F1-score while maintaining reasonable inference time. BERT and XLNet also performed well, but DistilBERT ranked the lowest in this evaluation due to its lower performance metrics. The TOPSIS method effectively ranked these models, providing a data-driven approach to selection.

**6. Future Work**
Additional factors such as training cost and domain-specific performance could be included in further analyses to refine model selection.

