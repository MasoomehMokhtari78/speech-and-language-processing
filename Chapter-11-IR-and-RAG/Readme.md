# Retrieval-Augmented Generation (RAG) & Dense Retrieval

This repository contains the presentation slides and academic materials for two comprehensive sessions covering the engineering principles, mathematical foundations, and advanced architectures of **Information Retrieval (IR)** and **Retrieval-Augmented Generation (RAG)**.

## 📘 Content Overview

The materials are systematically divided into two main components:

### 1. Book Presentation: Information Retrieval & Foundations of RAG

Based entirely on **Chapter 11 (Information Retrieval and Retrieval Augmented Generation)** from _Speech and Language Processing_ (3rd ed. draft) by Dan Jurafsky and James H. Martin.

- **Classic IR & Lexical Search:** Analysis of term weighting frameworks, specifically **TF-IDF** and **Okapi BM25**, alongside the mechanics of efficient text indexing via the **Inverted Index**.
- **IR Evaluation Metrics:** Comprehensive breakdown of unranked and ranked retrieval evaluation metrics, including **Precision**, **Recall**, **F-measure**, **Mean Average Precision (MAP)**, **Mean Reciprocal Rank (MRR)**, and **Normalized Discounted Cumulative Gain (NDCG)**.
- **Dense Retrieval & Neural IR:** Transitioning from sparse vector matching to dense embedding spaces. Covers **Bi-encoders** and **Cross-encoders** for semantic text matching, as well as token-level late-interaction architectures like **ColBERT** utilizing the MaxSim operator.
- **Foundational RAG Architecture:** The text's formulation of the two-stage "Retrieve-and-Read" pipeline, exploring how external text collections are leveraged by language models to satisfy factoid question answering and human information needs.

### 2. Paper Presentation: Seminal RAG Architecture & Deep Dive

Based on the groundbreaking NeurIPS research paper: _"Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks"_ (Lewis et al., 2020).

- **Parametric vs. Non-Parametric Memory:** Deep dive into RAG's core formulation—combining **Parametric Memory** (a pre-trained seq2seq BART transformer containing structural and language capabilities) with **Non-Parametric Memory** (a dense vector index of Wikipedia accessed via a Dense Passage Retriever (DPR)).
- **RAG-Sequence vs. RAG-Token Formulations:** \* **RAG-Sequence:** Uses the same retrieved document to condition and guide the generation of the entire target sequence.
- **RAG-Token:** Dynamically switches and samples from different documents on a per-token basis, synthesizing facts from disparate knowledge sources within a single output.

- **Knowledge Index Hot-Swapping:** Proof of architectural flexibility demonstrating how a model's world knowledge can be updated or substituted in real-time (e.g., swapping a 2016 Wikipedia index for a 2018 index) without retraining any model weights.
- **Knowledge-Intensive NLP Benchmarks:** Performance evaluations across Open-Domain QA (Natural Questions, TriviaQA, WebQuestions, CuratedTREC) and abstractive generation tasks (Jeopardy question generation and MS MARCO), highlighting substantial drops in hallucination.

---

## 🎥 Video Explanation

A complete recorded video walkthrough explaining the slides, mathematical equations, architectural comparisons, and training methodologies can be accessed here:

🎬 **[Watch the Presentation Video Recording Here](https://www.aparat.com/v/lid2mu7)**

---

## 🔗 Extra Resources & Further Reading

To expand your understanding of modern RAG systems, context engineering, and their evolution toward Agentic AI workflows, explore these curated resources:

### 🎓 Deep Dives & Architectural Long-Forms

- [RAG Explained: The Architecture Behind Agentic AI Systems](https://maven.com/p/85ea43/rag-explained-the-architecture-behind-agentic-ai-systems) — An intensive technical breakdown of the structural components empowering modern enterprise-grade AI agents.
- [RAG is the What. Agentic Search is the How](https://maven.com/p/7105dc) — A strategic guide exploring how simple document retrieval matures into adaptive, agent-driven search patterns.

### 📺 IBM Short Video Series on RAG

- [Is RAG Still Needed? Choosing the Best Approach for LLMs](https://www.youtube.com/watch?v=UabBYexBD4k) — A concise architectural debate assessing RAG alongside fine-tuning and long-context windows.
- [RAG's Evolution: From Simple Retrieval to Agentic AI](https://www.youtube.com/watch?v=JB2P5Gk23VI) — A historical and technical evolutionary chart mapping the journey from basic semantic matching to multi-hop autonomous agents.
- [How RAG, GraphRAG, and Context Engineering Improve AI Performance](https://www.youtube.com/watch?v=pN-LfxNFiTc) — A study of state-of-the-art context engineering practices and the integration of Knowledge Graphs (GraphRAG) to elevate factual consistency.

---

## 🤝 Acknowledgements

This presentation was done in the Tarbiat Modares University Computer Engineering Department, LLM in SE, professor Dr. Mahdie Ghasemi and presented by Masoomeh Mokhtari and Rashed Shahabi.
