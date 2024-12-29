# **MedLam: An Intelligent Medical Assistant**

MedLam is a research project focused on leveraging Large Language Models (LLMs) to enhance medical education and assistance. This tool is designed to aid medical students, professors, and doctors by providing reliable answers to medical queries, mentoring students, and streamlining teaching processes.

---

## **Overview**

MedLam explores the fine-tuning of LLMs using a Medical QA dataset to improve their performance for domain-specific tasks. By combining state-of-the-art natural language processing techniques and medical data, MedLam aims to deliver an effective and intuitive medical assistant.

---

## **Features**
- **Fine-Tuned LLMs**: Optimized large language models tailored for medical use cases.
- **Medical QA Dataset**: Processed and utilized datasets containing 100K+ records of medical queries and responses.
- **Custom LoRA Fine-Tuning**: Incorporates Low-Rank Adaptation (LoRA) techniques to enhance model performance efficiently.
- **Model Validation**: Comparison and validation of multiple models using key metrics like accuracy and F1-score.
- **Use Cases**:
  - Assisting medical students in understanding complex topics.
  - Supporting professors in teaching and curriculum design.
  - Helping doctors with quick and accurate responses to medical questions.

---

## **Project Architecture**

1. **Data Preparation**:
   - Preprocessed Medical QA datasets for training and evaluation.
2. **Model Fine-Tuning**:
   - Applied LoRA PEFT (Parameter-Efficient Fine-Tuning) to train LLMs on domain-specific data.
3. **Performance Validation**:
   - Analyzed and compared models across multiple configurations to determine optimal hyperparameters.
4. **Deployment (Future Scope)**:
   - Aimed at integrating the fine-tuned model into a user-friendly medical assistant platform.

---

## **Technologies Used**
- **Programming Languages**: Python  
- **Frameworks**: PyTorch, Hugging Face Transformers  
- **Machine Learning Techniques**: LoRA PEFT, Deep Learning  
- **Tools**: NumPy, Pandas, Sci-kit Learn  

---

## **Setup Instructions**
1. Clone this repository:
   ```bash
   git clone https://github.com/avishek04/MedLam.git

2. Navigate to the project directory:
   ```bash
   cd MedLam

4.	Run the training script:
   ```bash
   python train_model.py

5.	Evaluate the model:
   ```bash
   python evaluate_model.py
