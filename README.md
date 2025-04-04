# **MedLam: An Intelligent Medical Assistant**

MedLam is a research project focused on leveraging Large Language Models (LLMs) to enhance medical education and assistance. This tool is designed to aid medical students, professors, and doctors by providing reliable answers to medical queries, mentoring students, and streamlining teaching processes.

---
base_model: unsloth/Meta-Llama-3.1-8B-Instruct-bnb-4bit 

library_name: peft 

license: mit 

datasets:
- medalpaca/medical_meadow_medical_flashcards
- medalpaca/medical_meadow_mediqa
- medalpaca/medical_meadow_wikidoc
- medalpaca/medical_meadow_wikidoc_patient_information
- medalpaca/medical_meadow_mmmlu
- medalpaca/medical_meadow_pubmed_causal
- medalpaca/medical_meadow_health_advice
- ngram/medchat-qa
  
language: 
- en 

tags:
- medical
- biology
- chemistry
---

# Model Card for Model ID

<!-- Provide a quick summary of what the model is/does. -->

This Llama 3.1 8B Instruct Model was obtained using the Unsloth library. It is fine-tuned using the LoRA PEFT approach to give better responses to medical questions.

## Model Details

### Model Description

<!-- Provide a longer summary of what this model is. -->

MedLam explores the fine-tuning of LLMs using a Medical QA dataset to improve their performance for domain-specific tasks. By combining state-of-the-art natural language processing techniques and medical data, MedLam aims to deliver an effective and intuitive medical assistant.

- **Developed by:** Avishek Choudhury
- **Model type:** Transformer based auto-regressive language model
- **Language(s) (NLP):** English
- **License:** MIT
- **Finetuned from model Meta Llama 3.1 8B Instruct:** unsloth/Meta-Llama-3.1-8B-Instruct-bnb-4bit

### Model Sources

<!-- Provide the basic links for the model. -->

- **Repository:** https://github.com/avishek04/MedLam/tree/main
- **Paper:** https://arxiv.org/abs/2106.09685
<!-- - **Demo [optional]:** [More Information Needed] -->

## Uses

<!-- Address questions around how the model is intended to be used, including the foreseeable users of the model and those affected by the model. -->
This model was developed only for research and learning purposes and is not be meant for commercialization as a final product.

- Assisting medical students in understanding complex topics.
- Supporting professors in teaching and curriculum design.
- Helping doctors with quick and accurate responses to medical questions.

## How to Get Started with the Model

Use the code below to get started with the model.

```
from peft import PeftModel
from transformers import AutoModelForCausalLM

base_model = AutoModelForCausalLM.from_pretrained("unsloth/Meta-Llama-3.1-8B-Instruct-bnb-4bit")
model = PeftModel.from_pretrained(base_model, "aviici4cs/MedLam")
```

### Training Procedure

<!-- This relates heavily to the Technical Specifications. Content here should link to that section when it is relevant to the training procedure. -->
1. **Data Preparation**:
   - Preprocessed Medical QA datasets for training and evaluation.
2. **Model Fine-Tuning**:
   - Applied LoRA PEFT (Parameter-Efficient Fine-Tuning) to train LLMs on domain-specific data.
3. **Performance Validation**:
   - Analyzed and compared models across multiple configurations to determine optimal hyperparameters.
4. **Deployment (Future Scope)**:
   - Aimed at integrating the fine-tuned model into a user-friendly medical assistant platform.

#### Hardware

Google Colab

#### Software

- **Programming Languages**: Python  
- **Frameworks**: Unsloth Library, PyTorch, Hugging Face Transformers  
- **Machine Learning Techniques**: LoRA PEFT, Deep Learning  
- **Tools**: NumPy, Pandas, Sci-kit Learn  

## Model Card Contact
- https://www.linkedin.com/in/avishekchoudhury/
- https://github.com/avishek04
- https://avishek04.github.io/

### Framework versions

- PEFT 0.13.2
