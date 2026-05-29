# <center> 📰 ☣ ⚕ <font color = 'pink'>**Transformer-based biomedical text condensation**</font></center>

Biomedical text summarization project using transformer-based architectures to condense long-form scientific literature into concise and coherent summaries.

---

## 🧠 Problem Description

Scientific and biomedical papers often exceed the token limitations of transformer architectures, making direct summarization difficult.

This project explores token-aware chunking strategies combined with domain-adapted transformer models to generate high-quality summaries from long biomedical documents.

The experimentation focuses on evaluating summarization quality, coherence, and information retention using ROUGE metrics.

---

## 📊 Final Model Results

| Model     | ROUGE-1 | ROUGE-2 | ROUGE-L | ROUGE-Lsum |
| --------- | ------- | ------- | ------- | ---------- |
| BioBART   | 0.3480  | 0.0992  | 0.1787  | 0.1788     |
| BART      | 0.3484  | 0.1037  | 0.1802  | 0.1806     |
| Falconsai | 0.3669  | 0.1164  | 0.2022  | 0.2022     |

The evaluation compares multiple transformer-based summarization models on biomedical scientific articles using ROUGE metrics. Results suggest that Falconsai achieved the strongest overall summarization performance across all evaluated metrics.

---

## ⚙️ Requirements & Installation

```bash
pip install torch transformers datasets evaluate rouge-score gradio bitsandbytes sentencepiece accelerate
```

> Requires Python 3.10+

---

## 🚀 How to Run

```bash
git clone https://github.com/your-username/your-repo.git

cd your-repo

python app.py
```

---

## 📁 Project Structure

```bash
├── notebook.ipybn/
├── .gitignore/
├── experimentation_log.md
├── requirements.txt
└── README.md
```

---

## 🧪 Models Used

* facebook/bart-base
* GanjinZero/biobart-base
* Falconsai/text_summarization
---

## 📚 Dataset

* `ccdv/pubmed-summarization`

---

## 📈 Evaluation Metrics

* ROUGE-1
* ROUGE-2
* ROUGE-L
* ROUGE-Lsum

---

## 🎯 Objective

The goal of this project is to investigate how transformer-based summarization systems perform on long biomedical documents and how chunking strategies influence summary quality under token-length constraints.
