<!--
  ╔═══════════════════════════════════════════════════════════╗
  ║           ASHEESH DHAMACHARLA — GitHub Profile           ║
  ╚═══════════════════════════════════════════════════════════╝
-->

<div align="center">

```
█████╗ ███████╗██╗  ██╗███████╗███████╗███████╗██╗  ██╗
██╔══██╗██╔════╝██║  ██║██╔════╝██╔════╝██╔════╝██║  ██║
███████║███████╗███████║█████╗  █████╗  ███████╗███████║
██╔══██║╚════██║██╔══██║██╔══╝  ██╔══╝  ╚════██║██╔══██║
██║  ██║███████║██║  ██║███████╗███████╗███████║██║  ██║
╚═╝  ╚═╝╚══════╝╚═╝  ╚═╝╚══════╝╚══════╝╚══════╝╚═╝  ╚═╝
```

**`Building AI systems that actually ship.`**

*LLM Inference · Multimodal RAG · Agentic AI*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/asheeshdhamacharla)

![Visitors](https://komarev.com/ghpvc/?username=Asheesh07788&style=flat-square&color=6366f1)

</div>

---

## ⚖️ DIA-Legal — Multimodal RAG for Legal Proceedings

> *"What did the witness say about the gearbox at the 2011 Malaysia race?"*

A pipeline that makes courtroom video **queryable**. Ingest any legal proceeding — get speaker-attributed answers with timestamp-accurate citations.

```
Video → FFmpeg → WhisperX (diarization) → Chunks → CLIP + SentenceTransformers
     → LanceDB (MMR retrieval) → Cross-encoder reranking → LLM → Answer + Citations
```

**What makes it non-trivial:**
- Speaker attribution preserved end-to-end through chunking, embedding, and retrieval
- Adaptive alpha weighting — query type determines text vs visual retrieval balance
- Temporal expansion ±5s — automatically captures conversational context around evidence
- Confidence scoring across retrieval gap, normalized score, and coverage signals

`WhisperX` `LanceDB` `CLIP` `SentenceTransformers` `Gradio` `HuggingFace`

**[→ Live Demo](https://huggingface.co/spaces/Asheesh7/dia-legal_)** · **[→ Code](https://github.com/Asheesh07788/dia-legal)**

---

## ⚡ EAAD — Entropy-Aware Adaptive-K Speculative Decoding

> *Standard speculative decoding uses fixed k=4 draft tokens. Always. Regardless of how uncertain the model is. That's wasteful.*

Built an adaptive mechanism: **token-level entropy controls draft length.**

```python
entropy_bins = [0.5, 1.5, 2.5]
k_values     = [4,   3,   2,   1]

# High entropy → model uncertain → minimal drafting → no wasted compute
# Low entropy  → model confident → aggressive drafting → maximum speedup
```

**Result:** Up to 20-30% LLM inference latency reduction on Llama-2 7B.  
**Secondary finding:** Speculative output showed better diversity vs vanilla autoregressive decoding.

`PyTorch` `TinyLlama-1.1B` `Llama-2-7B` `HuggingFace Transformers` `Kaggle P100`

**[→ Code + Results](https://github.com/Asheesh07788/eaad)**

---

## 🌐 SentriX — Autonomous Supply Chain Risk Intelligence

> *Custom AI agents. Live signals. Zero human intervention per decision.*

Agents monitor **news + weather + financial markets** simultaneously → score disruption risk → recommend optimal shipping routes in real time.

```
Live Signals (News · Weather · Markets)
        ↓
  Custom Agent Loop
        ↓
  Risk Scoring Engine
        ↓
  Route Recommendation
```

Not a chatbot with tools. A decision intelligence system.

`GPT-4` `Custom Agents` `React` `Vercel`

**[→ Live App](https://sentri-x-t8bl.vercel.app/)** · **[→ Code](https://github.com/Asheesh07788/sentrix)**

---

## 🔬 Foundations

| Project | What It Proves |
|---|---|
| [Enterprise RAG from Scratch](https://github.com/Asheesh07788) | Built every RAG component without frameworks — embeddings, retrieval, reranking, generation |
| [GPT-2 from First Principles](https://github.com/Asheesh07788) | Implemented full transformer architecture — attention, positional encoding, training loop |

---

## 🛠 Stack

```
Language      Python  ████████████████████░

Inference     PyTorch · HuggingFace · TinyLlama · Llama-2 · Mistral
RAG           LanceDB · FAISS · SentenceTransformers · CLIP · LangChain
Multimodal    WhisperX · CLIP ViT-B/32 · FFmpeg
Agents        Custom Agent Loops · GPT-4 · Tool Use
Deploy        Gradio · FastAPI · Docker · Vercel · HuggingFace Spaces
```

---

## 📊 GitHub Stats

<div align="center">

![Asheesh's GitHub Stats](https://github-readme-stats.vercel.app/api?username=Asheesh07788&show_icons=true&theme=dark&hide_border=true&bg_color=0d1117&title_color=6366f1&icon_color=6366f1&text_color=e2e8f0)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=Asheesh07788&layout=compact&theme=dark&hide_border=true&bg_color=0d1117&title_color=6366f1&text_color=e2e8f0)

</div>

---

## 🎯 Currently

```python
status = {
    "building"   : "DIA-Legal v2 — better frame analysis + streaming ingestion",
    "exploring"  : "Speaker-attributed RAG as a research problem",
    "open_to"    : ["AI/ML Engineering", "Inference", "RAG", "Agentic AI"],
    "location"   : "Hyderabad, India — open to relocation",
    "graduating" : "April 2026",
}
```

---

<div align="center">

*If you're building real LLM products — inference infrastructure, RAG systems, agentic AI — let's talk.*

**[linkedin.com/in/asheeshdhamacharla](https://linkedin.com/in/asheeshdhamacharla)**

</div>
