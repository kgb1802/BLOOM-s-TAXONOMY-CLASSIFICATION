# 🎓 Bloom's Taxonomy Question Classifier

An end-to-end, privacy-first NLP application that automatically categorizes academic questions into the 6 cognitive complexity levels of Bloom's Taxonomy (*Remember*, *Understand*, *Apply*, *Analyze*, *Evaluate*, *Create*). 

Built using a fine-tuned **DistilBERT** transformer model, hardware-accelerated locally on Apple Silicon (M2 GPU via PyTorch MPS), and served through an interactive dual-mode **Streamlit** dashboard.

## 🌟 Key Features
- **Transformer Fine-Tuning**: Custom sequence classification head built on `distilbert-base-uncased` (66M parameters).
- **Edge GPU Acceleration**: Local training & inference leveraging Apple Silicon's Metal Performance Shaders (`torch.device("mps")`).
- **Interactive Single-Prompt Analysis**: Real-time predictions with full probability distribution progress bars across all 6 cognitive tiers.
- **Batch CSV Processing**: Bulk question classification for entire exam papers with one-click exportable CSV reports.
- **Zero-Cloud Dependency**: 100% local, privacy-focused execution with no API costs.

## 🛠️ Tech Stack
- **Language**: Python 3.12
- **Model & NLP**: Hugging Face `transformers`, `datasets`, PyTorch
- **Hardware Acceleration**: PyTorch MPS (Metal Performance Shaders)
- **Frontend / Interface**: Streamlit
- **IDE**: Visual Studio Code
