# Multi-Modal Advanced RAG Pipeline with Stateful Orchestration

An enterprise-grade, end-to-end Multi-Modal Retrieval-Augmented Generation (RAG) system engineered to ingest, analyze, and synthesize unstructured text and complex visual assets. The architecture features an autonomous state machine that dynamically routes queries, decomposes complex prompts, and applies deep re-ranking to deliver highly contextual, unified responses.

---

## 🚀 Key Features & Core Architecture

### 🧠 Stateful Multi-Agent Orchestration
* **Dynamic Workflow Routing:** Architected a robust state machine utilizing **LangGraph** to manage conversational state and dynamically route inputs between targeted RAG execution paths and general chat states based on real-time query intent classification.
* **Advanced Query Optimization:** Integrated query decomposition techniques to break down multi-faceted prompts into sub-problems, executing parallel retrievals for comprehensive answers.

### 👁️ Multi-Modal Information Synthesis
* **Visual-Textual Alignment:** Engineered true multi-modal capabilities by coupling deep semantic text retrieval with a local **BLIP (Bootstrapping Language-Image Pre-training)** vision transformer pipeline.
* **Unified Context Ingestion:** Developed a resilient asset-fetching infrastructure featuring specialized URL normalization and browser-emulated fallback layers to stream and process raw binary image payloads seamlessly.

### 🔍 High-Performance Search & Retrieval Engine
* **Scalable Vector Infrastructure:** Deployed a persistent **ChromaDB** vector database indexing over **1,000+ document chunks** to support high-density semantic searches.
* **Dense Embeddings & Re-ranking:** Utilized high-performance **384-dimensional sentence-transformer** embeddings to optimize semantic similarity spaces, backed by secondary document re-ranking algorithms to minimize context noise and combat LLM hallucination.
* **Automated Data Ingestion:** Built custom high-resiliency web scrapers to handle end-to-end data harvesting, sanitization, and automated pipeline ingestion.
