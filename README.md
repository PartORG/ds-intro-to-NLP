# Intro to NLP

In this repo, we will explore various topics related to Natural Language Processing (NLP), providing hands-on tutorials through Jupyter Notebooks. Each notebook builds upon the previous one, starting with basic text processing and moving through advanced models like Transformers for zero-shot learning.

## Features

### Comprehensive Tutorials
- **Spam Classifier**: Basic text processing and model training.
- **Zero Shot Learning**: Using pretrained networks from the Transformers library to predict spam.
- **Transformer Pipeline Models**: Exploring different models suitable for various NLP tasks.
- **Create Embeddings**: Understanding how embeddings are created for neural network models.

### Continuous Integration & Delivery
- Automated workflows for testing and deployment, ensuring that each notebook functions as expected.

## How It Works

The repository is structured around a series of Jupyter Notebooks designed to introduce users to various aspects of NLP. Each notebook builds upon the previous one, starting with basic text processing and moving through advanced models like Transformers for zero-shot learning. The tutorials are intended to be completed in pairs, following a specific order.

## Technology Stack

| Technology | Purpose |
|------------|---------|
| **TensorFlow** | Core library for building and training machine learning models. |
| **TensorFlow Hub** | Pretrained models and modules that can be easily integrated into TensorFlow applications. |
| **Scikit-learn** | Simple and efficient tools for data mining and data analysis, built on NumPy, SciPy, and matplotlib. |
| **Pandas** | Data structures and operations for manipulating numerical tables and time series. |
| **Seaborn** | A Python data visualization library based on Matplotlib that provides a high-level interface for drawing attractive statistical graphics. |
| **Statsmodels** | Provides classes and functions for the estimation of many different statistical models, as well as for conducting statistical tests, and statistical data exploration. |
| **JupyterLab** | An open-source web-based interactive development environment for Jupyter notebooks, code, and data. |
| **Pydot** | A Python interface to Graphviz’s Dot language. |
| **NLTK** | Natural Language Toolkit: a leading platform for building Python programs to work with human language data. |
| **SentencePiece** | A subword tokenizer and detokenizer. |
| **Transformers** | Hugging Face's library of pre-trained models, optimized for inference and training on various NLP tasks. |
| **IPyWidgets** | Interactive widgets for Jupyter notebooks. |
| **Testbook** | A tool to test Jupyter Notebooks. |
| **HDF5** | Hierarchical Data Format version 5, a file format designed to store large amounts of data and allows efficient access to that data. |

## Requirements

To run the tutorials in this repository, you will need:

- Python 3.11.3
- JupyterLab
- TensorFlow 2.16.2
- TensorFlow Hub 0.16.1
- Scikit-learn 1.5.1
- Pandas 2.2.2
- Seaborn 0.13.2
- Statsmodels 0.14.2
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

#### Step 1: Install Rust and HDF5

```bash
brew install rustup
rustup-init -y
# Choose the standard installation (press 1)
brew install hdf5
```

Restart your terminal and check the Rust version:

```bash
rustup --version
```

#### Step 2: Set up the virtual environment and install dependencies

For macOS with **silicon** chips:

```bash
pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements_silicon.txt
```

For macOS with **intel** chips:

```bash
pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

### WindowsOS

#### Step 1: Install Rust and HDF5

1. Visit the official Rust website: [https://www.rust-lang.org/tools/install](https://www.rust-lang.org/tools/install).
2. Download and run the `rustup-init.exe` installer.
3. Follow the on-screen instructions and choose the default options for a standard installation.

Then, install HDF5:

```bash
choco upgrade chocolatey
choco install hdf5
```

Restart your terminal and check the Rust version:

```bash
rustup --version
```

#### Step 2: Set up the virtual environment and install dependencies

For `PowerShell` CLI:

```powershell
pyenv local 3.11.3
python -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
```

For `Git-bash` CLI:

```bash
pyenv local 3.11.3
python -m venv .venv
source .venv/Scripts/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
```

## Configuration

No specific configuration files or environment variables are required for this repository.

## Quick Start

To get started, follow these steps:

1. Fork the repository.
2. Clone your fork to your local machine.
3. Set up a virtual environment as described in the installation section.
4. Open the Jupyter Notebooks in the order specified in the README.

## Usage

Each notebook provides detailed instructions and examples on how to use the tools and techniques covered in that tutorial. You can run each cell individually or execute the entire notebook to see the results.

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
│   │   ├── events.out.tfevents.1768233176.LEGION.311212.1.v2
│   │   ├── events.out.tfevents.1768233210.LEGION.311212.2.v2
│   │   ├── events.out.tfevents.1768233246.LEGION.311212.3.v2
│   │   ├── events.out.tfevents.1768235575.LEGION.311212.5.v2
│   │   ├── events.out.tfevents.1768235769.LEGION.311212.7.v2
│   │   ├── events.out.tfevents.1768235859.LEGION.311212.9.v2
│   │   ├── events.out.tfevents.1768235897.LEGION.311212.11.v2
│   │   ├── events.out.tfevents.1768235999.LEGION.311212.13.v2
│   │   ├── events.out.tfevents.1768236281.LEGION.311212.15.v2
│   │   ├── events.out.tfevents.1768236305.LEGION.311212.16.v2
│   │   └── events.out.tfevents.1768236347.LEGION.311212.17.v2
│   └── validation/
│       ├── events.out.tfevents.1768233248.LEGION.311212.4.v2
│       ├── events.out.tfevents.1768235577.LEGION.311212.6.v2
│       ├── events.out.tfevents.1768235772.LEGION.311212.8.v2
│       ├── events.out.tfevents.1768235860.LEGION.311212.10.v2
│       ├── events.out.tfevents.1768235899.LEGION.311212.12.v2
│       ├── events.out.tfevents.1768236001.LEGION.311212.14.v2
│       └── events.out.tfevents.1768236349.LEGION.311212.18.v2
├── metadata.tsv
└── requirements.txt
```

## Development

The repository includes workflows for continuous integration and delivery, as well as scripts for managing issues and pull requests.

## Testing

No specific tests are included in this repository.

## Limitations

- The tutorials assume a basic understanding of Python and machine learning concepts.
- Some notebooks may require additional setup or dependencies not listed here.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.