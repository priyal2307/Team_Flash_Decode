# 🚀 LLM Inference Pipeline Accelerator 

**Computer Architecture Project**

A cycle-level simulator for analyzing and optimizing **LLM (Large Language Model) inference performance**, with a focus on memory hierarchy, compute throughput, and modern attention optimizations.

---

## 📌 Overview

This project models the **token generation pipeline of transformer-based LLMs** at a cycle level, enabling detailed analysis of:

* Compute vs memory bottlenecks
* SRAM vs HBM bandwidth usage
* KV-cache behavior
* Throughput and latency trade-offs
* Advanced decoding optimizations

The simulator integrates modern research techniques such as **FlashAttention, speculative decoding, and continuous batching**.

---

## ⚙️ Features

### ✅ Core Functionality

* Cycle-level simulation of transformer inference
* Accurate **cycles per token** computation
* Memory traffic modeling (SRAM vs HBM)
* Energy estimation based on hardware parameters

### 🛠️ Improvements & Enhancements

* Prefill + decode phase modeling (TTFT support)
* KV-cache scaling across layers
* Hardware-aware throughput simulation
* Analytical DMA overlap modeling

### 🔬 Advanced Techniques Implemented

* FlashAttention / FlashDecoding models
* Speculative decoding (Leviathan et al. 2023)
* Continuous batching (vLLM-style)
* GQA / MQA attention variants
* KV-parallelism strategies

---

## 🧠 Key Concepts

* **Roofline Model** for performance analysis
* **Memory-bound vs compute-bound workloads**
* **Transformer attention optimizations**
* **Hardware-aware simulation**

---

## 📂 Project Structure

```
.
├── Team_Flash_Decode.ipynb   # Main simulation notebook
├── Outputs                   # Output images
├── README.md                 # Project documentation
```

---

## ▶️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPO.git
cd YOUR_REPO
```

2. Install dependencies:

```bash
pip install matplotlib numpy
```

3. Run the notebook:

```bash
jupyter notebook
```

Open:

```
Team_Flash_Decode.ipynb
```

---

## 📊 Outputs

The simulator generates:

* Throughput vs batch size plots
* Latency breakdown (prefill vs decode)
* Memory bandwidth utilization
* Performance comparisons across techniques

---

## 📚 References

* Williams et al. (2009) — Roofline Model
* Dao et al. (2022–2024) — FlashAttention series
* Kwon et al. (2023) — vLLM / PagedAttention
* Leviathan et al. (2023) — Speculative Decoding
* Ainslie et al. (2023) — GQA
* Shazeer (2019) — MQA
* MLPerf Inference v4.0 (2024)

---

## 🎯 Goals

* Understand LLM inference bottlenecks
* Explore hardware/software co-design
* Evaluate modern optimization strategies
* Provide a research-oriented simulation framework

---

## 👥 Team

**Team Flash Decode**

Priyal Chiragbhai Shah - 035255452
Shlok Kaushikbhai Patel - 035257987

---

## 📌 Future Work

* GPU-specific kernel modeling
* Integration with real LLM frameworks
* Distributed inference simulation
* Support for quantization (INT4/FP8)

---

## 📄 License

This project is for academic and educational purposes.

---

## ⭐ Acknowledgements

Inspired by recent advancements in efficient LLM inference and open research in systems + ML.
