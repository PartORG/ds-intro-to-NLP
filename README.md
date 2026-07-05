# Intro to NLP

In this repo, we will explore various topics related to Natural Language Processing (NLP), including text classification, zero-shot learning, transformer pipeline models, and embedding creation. This project is designed for individuals looking to gain a comprehensive understanding of NLP techniques using popular libraries such as TensorFlow, PyTorch, and Hugging Face's Transformers.

## Table of Contents

- [Features](#features)
- [How It Works](#how-it-works)
- [Technology Stack](#technology-stack)
- [Requirements](#requirements)
- [Installation](#installation)
- [Configuration](#configuration)
- [Quick Start](#quick-start)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Development](#development)
- [Testing](#testing)
- [Limitations](#limitations)
- [License](#license)

## Features

### Text Classification
- **Spam Classifier**: Train a model to classify text as spam or not spam.
- **Zero Shot Learning**: Use pre-trained models for tasks without explicit training data.

### Transformer Pipeline Models
- **Transformers Zero Shot Pipeline**: Explore different transformer-based models for various NLP tasks.

### Embedding Creation
- **Create Embeddings**: Learn how to create embeddings for neural network models using TensorFlow and Hugging Face's Transformers.

## How It Works

This project is structured around a series of Jupyter notebooks that guide you through the process of building and deploying NLP models. Each notebook focuses on a specific aspect of NLP, from basic text processing to advanced transformer-based models.

## Technology Stack

| Technology | Purpose |
|------------|---------|
| TensorFlow | Core library for machine learning and deep learning. |
| PyTorch | Another popular deep learning framework. |
| Hugging Face Transformers | Pre-trained models and tools for natural language understanding. |
| Scikit-learn | Machine learning library for data mining and data analysis. |
| Pandas | Data manipulation and analysis library. |
| Seaborn | Statistical data visualization library based on Matplotlib. |
| Statsmodels | Statistical modeling and testing library. |
| JupyterLab | Interactive development environment for notebooks, code, and data. |
| Pydot | Python interface to Graphviz's Dot language. |
| NLTK | Natural Language Toolkit for text processing. |
| SentencePiece | Subword tokenization library. |
| IPyWidgets | Interactive widgets for Jupyter notebooks. |
| Testbook | Library for testing Jupyter notebooks. |
| HDF5 | Hierarchical Data Format for storing and managing large datasets. |

## Requirements

- Python 3.11
- TensorFlow 2.16.2
- TensorFlow-Hub 0.16.1
- Scikit-learn 1.5.1
- Pandas 2.2.2
- Seaborn 0.13.2
- Statsmodels 0.14.2
- JupyterLab 4.2.3
- Pydot 2.0.0
- NLTK 3.8.1
- SentencePiece 0.1.99
- Transformers 4.38.2
- IPyWidgets 8.0.6
- Testbook 0.4.2
- HDF5

## Installation

To set up your environment, follow these steps:

### macOS

```bash
# Step 1: Install rustup and hdf5
brew install rustup
rustup-init -y
brew install hdf5

# Step 2: Set up virtual environment and install packages
pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements_silicon.txt
```

### WindowsOS

#### PowerShell CLI

```powershell
# Step 1: Install rustup and hdf5
Invoke-WebRequest -Uri "https://www.rust-lang.org/install" -OutFile "rustup-init.exe"
.\rustup-init.exe
choco upgrade chocolatey
choco install hdf5

# Step 2: Set up virtual environment and install packages
pyenv local 3.11.3
python -m venv .venv
.venv\Scripts\Activate.ps1
pip install --upgrade pip
pip install -r requirements.txt
```

#### Git-bash CLI

```bash
# Step 1: Install rustup and hdf5
curl https://sh.rustup.rs -sSf | sh
choco upgrade chocolatey
choco install hdf5

# Step 2: Set up virtual environment and install packages
pyenv local 3.11.3
python -m venv .venv
source .venv/Scripts/activate
pip install --upgrade pip
pip install -r requirements.txt
```

## Configuration

No specific configuration is required for this project.

## Quick Start

To get started, follow these steps:

1. Fork the repository.
2. Clone your forked repository to your local machine.
3. Set up a virtual environment and install dependencies as described in the [Installation](#installation) section.
4. Open the Jupyter notebooks in the order specified in the [README.md](README.md).

## Usage

Run the Jupyter notebooks to explore each topic:

- **1_Spam_Classifier.ipynb**: Basic text processing and spam classification model training.
- **2_Spam_Zero_Shot.ipynb**: Zero-shot learning for spam prediction using pre-trained models.
- **3_Transformers_Zero_Shot_Pipeline.ipynb**: Exploring transformer-based models for various NLP tasks.
- **4_create_embeddings.ipynb**: Creating embeddings for neural network models.

## Project Structure

```
ds-intro-to-NLP/
├── .github/workflows/
│   ├── REGX_test_import_libraries.sh
│   ├── add_issue_to_done.yml
│   ├── add_issue_todo.yml
│   ├── add_pr_in_progress.yml
│   ├── add_pr_to_done.yml
│   ├── discord-webhook-notify.yml
│   ├── replacement.yml
│   └── testing/extra/utility.py
├── .gitignore
├── 1_Spam_Classifier.ipynb
├── 2_Spam_Zero_Shot.ipynb
├── 3_Transformers_Zero_Shot_Pipeline.ipynb
├── 4_create_embeddings.ipynb
├── 5_Optional.ipynb
├── LICENSE
├── README.md
├── data/
│   ├── SMSSpamCollection.txt
│   └── sample.csv
├── embeddings_output/
│   └── embedding.txt
├── extra/
│   └── utility.py
├── logs/
│   ├── train/
│   │   ├── events.out.tfevents.1768233138.LEGION.311212.0.v2
│   │   ├── ...
│   │   └── events.out.tfevents.1768236349.LEGION.311212.18.v2
│   └── validation/
│       ├── events.out.tfevents.1768233248.LEGION.311212.4.v2
│       ├── ...
│       └── events.out.tfevents.1768236349.LEGION.311212.18.v2
├── metadata.tsv
├── requirements.txt
├── requirements_silicon.txt
└── vectors.tsv
```

## Development

This project is open-source and contributions are welcome. If you find any issues or have suggestions for improvements, please submit a pull request.

## Testing

No tests are included in this repository.

## Limitations

- The project assumes basic knowledge of Python and machine learning.
- Some notebooks may require additional setup depending on your environment.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.