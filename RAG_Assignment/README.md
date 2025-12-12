# 📘 Retrieval-Augmented Generation (RAG) Learning Lab

_A hands-on teaching module for INFO 7390 – Advanced Data Science & Architecture_


🎥 Project Demo & Explanation Videos
------------------------------------

The following videos demonstrate the Retrieval-Augmented Generation (RAG) system from multiple perspectives, including a full walkthrough, a conceptual storytelling explanation, and a short-form AI-generated explainer.

### 📺 Screen Recording — Full System Walkthrough (VEED)

A detailed screen recording that walks through the notebook implementation, explaining each stage of the RAG pipeline, including document ingestion, chunking, embedding, retrieval, and grounded generation.

*   **YouTube:**👉 [Watch the full walkthrough](https://youtu.be/MjZJ504GH30)
    

### 📖 Story-Style Concept Explanation — RAG using NotebookLLM

A narrative, story-driven explanation of Retrieval-Augmented Generation designed to build intuition around how retrieval and generation work together.

*   **YouTube:**👉 [Watch the RAG story explanation](https://youtu.be/dxeSDckNEsE)
    

### ⚡ Short-Form AI-Generated Explainer — QuickFrame AI (15 seconds)

A concise, visually driven explainer video generated using QuickFrame AI that summarizes the core idea of RAG in a short, engaging format.

*   **QuickFrame Preview:**👉 [View the 15-second AI-generated video](https://ai.quickframe.com/preview/55d8c6bb-0820-43ba-81be-2c40533e2c13)

## 🎯 Overview

This repository is an **end-to-end educational package** designed to teach students the full workflow of **Retrieval-Augmented Generation (RAG)** — one of the most important design patterns in modern AI systems.

Learners build a complete **PDF Question-Answering system** using:

- Document loading
- Chunking strategies
- Embedding models
- Vector similarity search
- RAG prompt construction
- LLM grounding using OpenAI
- Evaluation, debugging, and visualization tools

The repository includes:

- A full tutorial notebook
- Starter code for learners
- Exercises with increasing difficulty
- Visualizations to interpret retrieval behavior
- Multi-document support
- Thresholding and similarity analysis
- End-to-end pipeline students can extend into production systems

This project is designed to **teach RAG by building RAG**.

## 🧠 What This Teaching Module Covers

### **✔ Core Concepts**

- Why RAG is needed
- Limitations of pure LLMs (hallucinations, context limits, outdated training)
- Embeddings & vector spaces
- Cosine similarity and nearest neighbor search
- Chunking strategies (size, overlap, quality tradeoffs)
- Prompt engineering for grounded generation

### **✔ Practical Implementation**

- Load and read text from multiple PDFs
- Split documents into overlapping semantic chunks
- Embed chunks using sentence-transformers
- Build a lightweight in-memory vector database
- Retrieve relevant context based on user questions
- Feed context into OpenAI’s Chat Completions API
- Evaluate answer groundedness

### **✔ Advanced Learning Features**

- **Exercise 1:** Chunk size and overlap exploration
- **Exercise 2:** Multi-document retrieval behavior
- **Exercise 3:** Similarity threshold tuning
- **Visualization:** Similarity distributions, multi-PDF retrieval, threshold effects

These exercises transform the notebook into a **guided laboratory experience**.

## 📁 Repository Structure

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`  ├── README.md                     # You are here  ├── rag.ipynb                     # Full teaching notebook  ├── starter_template.ipynb        # Learner version with TODOs  ├── data/  │   └── sample_papers/            # PDFs used for RAG  ├── tutorial/  │   └── rag_tutorial.md           # Theory + implementation walkthrough  ├── report/  │   └── pedagogical_report.pdf    # 6–10 page analysis (for submission)  ├── src/ (optional)  │   ├── pdf_loader.py  │   ├── text_splitter.py  │   ├── embeddings.py  │   ├── vector_store.py  │   └── rag_pipeline.py  └── requirements.txt  `

## 🚀 Quickstart

### 1️⃣ Install dependencies

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`  pip install -r requirements.txt  `

### 2️⃣ Add PDFs

Place your documents into:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`  data/sample_papers/  `

### 3️⃣ Run the notebook

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`  rag.ipynb  `

You'll be guided through:

- Loading PDFs
- Chunking
- Embedding
- Retrieval
- RAG prompting
- Answer generation

And finally, visualizing how your system makes decisions.

## 🎥 Show-and-Tell Video Structure

Your video should follow:

### **1\. Explain — What is RAG and Why Does It Matter?**

- Limitations of pure LLMs
- Motivation for retrieval
- Real-world applications

### **2\. Show — Live Walkthrough in the Notebook**

- Load PDFs
- Chunking & embedding
- Retrieve relevant context
- Call the LLM
- Visualize retrieval

### **3\. Try — Guided Exercises for Viewers**

- Modify chunk sizes
- Include multiple PDFs
- Add similarity thresholds
- Observe impact on accuracy

This aligns perfectly with the assignment’s **Explain → Show → Try** pedagogy.

## 📊 Visualizations Included

The notebook includes multiple visual diagnostic tools:

- Similarity bar plots
- Multi-document retrieval heatmaps
- Threshold cutoff visualizations
- Retrieval ranking scatter plots

These help students _see_ how RAG behaves, not just use it.

## 🧩 Learning Outcomes

Upon completing this module, a student will be able to:

- Describe RAG architecture and components
- Implement a minimal RAG system from scratch
- Evaluate retrieval strategies
- Debug RAG outputs and improve grounding
- Understand chunking and similarity tradeoffs
- Extend RAG to multiple documents and different models

This prepares them not only for academic understanding but for practical implementation in industry-grade AI systems.

## 💡 Extensions for Advanced Learners

Students can take this further by:

- Using FAISS, Pinecone, Weaviate
- Adding metadata filtering
- Using semantic chunking instead of word-based
- Implementing rerankers (cross-encoders)
- Building a Streamlit UI (“Chat with your PDFs”)
- Evaluating RAG with QA benchmarks

## 📘 Academic Integrity

AI tools were used for drafting, design assistance, and code debugging.All core implementation, structuring, and conceptual explanation were performed manually and are fully understood by the author.


📘 Academic Integrity & Use of AI Tools
---------------------------------------

This project was completed in accordance with the academic integrity guidelines of INFO 7390: Advanced Data Science and Architecture.

### Use of AI Assistance

AI tools (including large language models and generative media platforms) were used in this project in a **supportive and assistive capacity**, not as a substitute for original thought or understanding. Specifically, AI was used for:

*   Code debugging and refactoring assistance
    
*   Generating synthetic examples and edge-case scenarios
    
*   Drafting and refining explanatory text and documentation
    
*   Creating visual assets and short-form explainer videos
    
*   Improving clarity, structure, and presentation of written materials
    

All architectural decisions, system design choices, and instructional structure were conceived, implemented, and validated by the author.

### Original Work and Understanding

The core contributions of this project—including:

*   Selection of the Retrieval-Augmented Generation (RAG) concept
    
*   Design of the end-to-end RAG pipeline
    
*   Implementation of document ingestion, chunking, embedding, retrieval, and generation
    
*   Development of exercises, visualizations, and debugging workflows
    
*   Pedagogical framing and instructional narrative
    

represent original work. The author fully understands and can explain every component of the system, as demonstrated through the implementation, documentation, and accompanying video walkthroughs.

### AI-Generated Media

Some explanatory videos were generated using AI-based video tools for educational and illustrative purposes. These videos complement, but do not replace, the author’s own technical walkthroughs and conceptual explanations.

### Compliance Statement

This project adheres to the course policy permitting AI tools for:

*   Assistance with coding and debugging
    
*   Content generation for explanatory or illustrative purposes
    
*   Proofreading and formatting support
    

while maintaining full accountability for correctness, originality, and conceptual understanding.

## 🏁 Conclusion

This repository serves as a **self-contained RAG learning environment**, built for both beginners and advanced students. It blends theory, implementation, visualization, and experimentation into a cohesive teaching experience.

