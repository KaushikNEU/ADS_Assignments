# **Generative AI Coursework – Crash Course, Worked Examples & Quiz Assignment**
### *INFO 7390 – Art and Science of Data*  
### *Author: Kaushik Jayaprakash.*

---

## 📘 **Overview**

This repository contains all deliverables for the Generative AI coursework completed as part of INFO 7390. It includes:

- A **Crash Course in Generative AI** Jupyter Notebook  
- A **Dynamic Webpage Demo** for text generation  
- Two **Worked Examples** using GPT-2 on different datasets  
- A **One-Page Report** summarizing findings  
- A **15-Question Quiz Set** assessing conceptual understanding  

This repo demonstrates a complete progression from foundational theory → implementation → evaluation → assessment.

---

# 🧠 **Part 1 — Crash Course in Generative AI**

### **Notebook:** `Crash_Course_Generative_AI.ipynb`

This notebook introduces the foundations of generative AI, including:

- GANs, VAEs, Transformers, Diffusion Models  
- Self-attention, positional encoding, latent spaces  
- Training challenges and evaluation metrics  
- Practical demonstrations using Transformers  
- Visualizations and generated samples  
- Conclusions and references  

This notebook establishes the conceptual base for the worked examples.

---

# 🌐 **Part 2 — Dynamic Webpage Demonstration**

### **File:** `/Webpage_Demo/index.html`

An interactive webpage was created using HTML/CSS/JavaScript with the help of Replit’s AI coding assistant.

### **Features**
- User text input box  
- GPT-style text completion  
- Clean UI layout  
- Includes the AI-generated code and subsequent manual refinements  
- Screenshots documenting prompt engineering are included  

### **Hosting**
The webpage is deployed through **Replit Hosting** for live interaction.

---

# 🧪 **Part 3 — Worked Example 1 & 2: Generative Text Modeling**

### **Notebook:** `Worked_Examples_Text_Generation.ipynb`

This notebook implements two complete generative modeling examples using GPT-2.

---

## **Worked Example 1 — Wikitext-2 (Formal Writing)**

This example demonstrates:

- Text preprocessing and BPE tokenization  
- GPT-2 fine-tuning using causal language modeling  
- Validation loss and perplexity evaluation  
- Sample generation in formal, encyclopedic style  

**Key Insight:**  
GPT-2 adapts strongly to structured, formal text and maintains topic coherence.

---

## **Worked Example 2 — Reddit TIFU (Informal Storytelling)**

This example applies the same pipeline to informal, narrative-style user posts.

- Preprocessing and tokenization  
- GPT-2 fine-tuning  
- Higher perplexity due to noisy, conversational structure  
- Generated samples resemble personal anecdotes and casual storytelling  

**Key Insight:**  
Dataset style directly determines linguistic output—tone, phrasing, structure, and creativity.

---

## **Comparison Between Datasets**

- **Wikitext-2** → Lower perplexity, formal and structured text  
- **Reddit TIFU** → Higher perplexity, informal and expressive text  
- Same model → Different linguistic behavior due solely to dataset characteristics  

This highlights the importance of data selection in generative AI development.

---

## **Report**

A one-page written report summarizing dataset choices, methodology, comparative results, and key findings is included as part of the Canvas submission.

---

# 📝 **Part 4 — Quiz Section (15 Multiple-Choice Questions)**

A set of **15 MCQs** was created based on the Book Chapter topic:

### **Topic:** *Transformer-Based Text Generation Using GPT Models*

The quiz includes:

- 5 recall questions  
- 5 application questions  
- 5 analysis/evaluation questions  
- Correct answers with detailed explanations  
- References to specific sections/pages  

This demonstrates understanding of architecture, training techniques, decoding strategies, evaluation, and limitations.

---

# 📂 **Repository Structure**

/Crash_Course_Generative_AI.ipynb
/Worked_Examples_Text_Generation.ipynb
/Webpage_Demo/
└── index.html
/screenshots/
/Quiz_Questions.pdf (optional export)
README.md


---

# 📌 **How to Run the Code**

### **Jupyter Notebooks**
```bash
pip install transformers datasets torch

Open the notebooks in Jupyter or VS Code and run sequentially.

Webpage Demo

Open index.html in any browser or use the deployed Replit link.






