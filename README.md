# 🧠 End-to-End NLP Text Summarizer with Hugging Face Transformers

This project is a complete, production-ready implementation of an **Abstractive Text Summarization System** using state-of-the-art Transformer models (like T5 or BART) from Hugging Face 🤗. It follows a modular pipeline structure with YAML-based configuration, custom logging, and stage-wise development inspired by a professional NLP workflow.

---

## 🎯 Objective

To fine-tune a pretrained Transformer model for summarizing long text documents and expose it via an API for inference.

---

## 📦 Features

- ✅ Logging and Utility Management
- ✅ Hugging Face Transformers-based fine-tuning
- ✅ Modular ML pipeline (Ingestion → Transformation → Training → Evaluation → Inference)
- ✅ FastAPI-based REST endpoint
- ✅ YAML-driven configuration
- ✅ Docker support for easy deployment
- ✅ Jupyter notebooks for experimentation

---

## 📂 Project Structure

```
textsummarizer/
│
├── app.py                         # FastAPI app
├── main.py                        # Entry point to run full pipeline
├── Dockerfile                     # For containerization
├── config/                        # YAML configuration files
├── params.yaml                    # Model parameters
├── setup.py                       # Installable package setup
├── requirements.txt               # Project dependencies
├── research/                      # Experiment notebooks
├── src/textSummarizer/           # Core package
│   ├── components/               # Data ingestion, transformation, trainer, evaluator
│   ├── config/                   # Config parser
│   ├── constants/                # Static global values
│   ├── entity/                   # Data schemas
│   ├── logging/                  # Custom logging setup
│   ├── pipeline/                 # Stage-wise runner scripts
│   └── utils/                    # Helper functions
└── README.md
```

---

## 🧠 Based On Course Sections

| Course Topic                                   | Implemented |
| ---------------------------------------------- | ----------- |
| 159. Intro to Hugging Face & Problem Statement | ✅           |
| 160. GitHub Setup & Structure                  | ✅           |
| 161. Logging and Utils                         | ✅           |
| 162. Fine-tuning on Google Colab               | ✅           |
| 163-164. Data Ingestion                        | ✅           |
| 165. Data Transformation                       | ✅           |
| 166. Model Trainer                             | ✅           |
| 167. Model Evaluation                          | ✅           |
| 168. Prediction + API Integration              | ✅           |

---

## ⚙️ Installation

```bash
git clone https://github.com/yourusername/textsummarizer.git
cd textsummarizer
pip install -r requirements.txt
```

---

## ▶️ Usage

### Run the full pipeline:

```bash
python main.py
```

### Launch API:

```bash
uvicorn app:app --reload
```

Open: `http://127.0.0.1:8000/docs` for Swagger UI.

---

## 🐳 Docker

Build and run using Docker:

```bash
docker build -t textsummarizer .
docker run -p 8000:8000 textsummarizer
```

---

## 🧪 Jupyter Notebooks

Explore the `research/` directory for development steps:

- `1_data_ingestion.ipynb`
- `2_data_transformation.ipynb`
- `3_model_trainer.ipynb`
- `4_model_evaluation.ipynb`

---

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file.

---
s
## 👨‍💻 Author

Jeevan Aher

Masters of Science In computer Science  Student\
University of Illinois Springfield\
[LinkedIn](https://www.linkedin.com/in/jeevanaher732/)
