# 🎬 CineMatch AI

**BERT-Powered Movie Recommendation System**

## Features

- 🧠 **Hybrid Recommendation Engine**  
  Combines BERT embeddings with collaborative filtering
- ❄️ **Cold Start Solution**  
  Handles new users/movies effectively
- ⚡ **Real-Time Predictions**  
  <1s response time for recommendations
- 📊 **Context-Aware Analysis**  
  Understands themes, tones, and narrative styles

## Tech Stack

**Core Technologies**  
`Python 3.9` | `PyTorch` | `BERT` | `Transformers` | `scikit-learn`  

**Data Pipeline**  
`Pandas` | `NumPy` | `TF-IDF` | `Cosine Similarity`
## System Architecture

```mermaid
graph TD
    A[User Input] --> B{BERT Engine}
    B --> C[Content-Based Filtering]
    A --> D[Collaborative Filtering]
    C --> E[Hybrid Recommendations]
    D --> E

    style A fill:#FF4D6D,color:white
    style B fill:#4361EE,color:white
    style C fill:#FF9E00,color:black
    style D fill:#FF9E00,color:black
    style E fill:#2E7D32,color:white

    classDef process fill:#f0f0f0,stroke:#333,stroke-width:2px;
    classDef decision fill:#4361EE,color:white;
    classDef input fill:#FF4D6D,color:white;
    classDef output fill:#2E7D32,color:white;

    class A input
    class B decision
    class C,D process
    class E output
