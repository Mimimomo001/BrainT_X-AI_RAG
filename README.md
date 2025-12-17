# BrainT_XAI_RAG
Explainable Brain Tumor Detection with Visual RAG. An end-to-end Vision AI system for brain tumor identification from MRI scans, integrating deep learning, explainable AI (X-AI), and Visual Retrieval-Augmented Generation (Visual RAG) to provide interpretable, clinically grounded predictions. Unlike traditional CNN-only approaches, this project goes beyond classification by explaining why the model makes a decision, using both visual evidence (Grad-CAM) and retrieved medical knowledge.

## Model Training Details
- Backbone: EfficientNet-B3 (pretrained)
- Loss: Binary Cross-Entropy with Logits + Label Smoothing
- Optimizer: AdamW
- Regularization:
  - Dropout (0.7)
  - Weight decay
- Training Strategy:
  - Stage 1: Frozen backbone
  - Stage 2: Fine-tuning
  - Early stopping based on validation ROC-AUC
## Final validation metrics:
  loss: 0.2859
  
  acc: 0.9151
  
  precision: 0.9289
  
  recall: 0.9310
  
  f1: 0.9299
  
  auc: 0.9700

<img width="1182" height="380" alt="image" src="https://github.com/user-attachments/assets/2d5ba71c-b7a4-46cf-97aa-c510c7cd86a7" />
# Explainability example:
<img width="912" height="387" alt="image" src="https://github.com/user-attachments/assets/fbb7aab2-0e72-4cd2-b94b-ac181b6257f6" />
