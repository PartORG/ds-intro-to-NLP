# Intro to NLP

Explore various NLP topics through interactive Jupyter Notebooks.

## Requirements

To run this project, you need the following dependencies:

- Python 3.11.3
- TensorFlow 2.16.2
- TensorFlow-Hub 0.16.1
- TensorFlow-Docs
- Scikit-Learn 1.5.1
- Pandas 2.2.2
- Seaborn 0.13.2
- Statsmodels 0.14.2
- JupyterLab 4.2.3
- Pydot 2.0.0
- NLTK 3.8.1
- SentencePiece 0.1.99
- Transformers 4.38.2
- IPywidgets 8.0.6
- Testbook 0.4.2
- H5py 3.11.0

## Installation

### macOS (Intel)

```sh
pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

### macOS (Silicon)

```sh
pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements_silicon.txt
```

### Windows

For PowerShell CLI:

```PowerShell
pyenv local 3.11.3
python -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
```

For Git-bash CLI:

```BASH
pyenv local 3.11.3
python -m venv .venv
source .venv/Scripts/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
```

## Usage

Run the Jupyter Notebooks in the following order:

1. [Spam Classifier](1_Spam_Classifier.ipynb)
2. [Zero Shot Learning](2_Spam_Zero_Shot.ipynb)
3. [Transformer Pipeline Models](3_Transformers_Zero_Shot_Pipeline.ipynb)
4. [Create Embeddings](4_create_embeddings.ipynb)
5. [Optional](5_Optional.ipynb)

Each notebook covers different aspects of NLP, from basic text processing to advanced models and embeddings.