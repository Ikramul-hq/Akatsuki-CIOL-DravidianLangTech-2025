# Akatsuki-CIOL@DravidianLangTech 2025: Fake News Detection in Malayalam

This repository contains the implementation for the paper **"Ensemble-Based Approach Using Pre-Trained Models for Fake News Detection in Dravidian Languages"**, addressing the shared tasks at DravidianLangTech 2025. The study focuses on detecting fake news in Malayalam, a low-resource language, using transformer-based models and ensemble techniques.

## Key Details

### Tasks
1. **Task 1 (Binary Classification)**: Distinguish social media posts as *Fake* or *Original*.
   - **Dataset**: 3,257 training, 815 validation, 1,019 test samples.
   - **Model**: Fine-tuned `malayalam-bert-FakeNews-Dravidian` (M-BERT-Dravidian) with MLP classifier.
   - **Result**: Macro F1 score of **0.814** (ranked 14th in the competition).

2. **Task 2 (Multiclass Classification)**: Categorize Malayalam news articles into five classes (*False, Half True, Mostly False, Partly False, Mostly True*).
   - **Dataset**: 1,615 training, 285 validation, 200 test samples.
   - **Model**: Multimodal ensemble of `L3Cube-BERT` and `MuRIL` embeddings.
   - **Result**: Macro F1 score of **0.1978** (ranked 11th), highlighting challenges in nuanced classification.

### Methodology
- **Preprocessing**: Tokenization, padding/truncation (512 tokens for Task 1, 128 for Task 2), and oversampling to address class imbalance.
- **Architecture**: 
  - **Task 1**: BERT-based model with MLP (hidden layers: 786, 512 dimensions).
  - **Task 2**: Combined embeddings from multiple pre-trained models for enhanced contextual understanding.
- **Training**: Adam optimizer (LR=0.0001), batch size=16, dropout=20% (Task 1).

### Key Findings
- **Task 1** achieved strong performance due to balanced data and effective fine-tuning.
- **Task 2** struggled with class imbalance, dialectal variations, and subtle semantic distinctions between labels (e.g., "Half True" vs. "Partly False").
- Ensemble models improved robustness but increased computational complexity.

### Challenges & Future Work
- **Limitations**: Small datasets, bias risks from oversampling, and reliance on pre-trained models.
- **Recommendations**: Larger datasets, explainable AI techniques, and zero-shot learning for low-resource settings.

## Impact
This work advances fake news detection in underrepresented languages, promoting equitable AI solutions. By addressing linguistic diversity and code-mixing, it lays the groundwork for scalable misinformation mitigation in Malayalam and other Dravidian languages.

---

**Paper Reference**: [Akatsuki-CIOL@DravidianLangTech 2025](CWMLB___T1_Akatsuki_CIOL.pdf)  
**Contact**: Azmine Toushik Wasi (`azmine32@student.sust.edu`)
