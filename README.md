
# BLP25-Task1: Hate Speech Identification

This repository contains the code and dataset for the BLP25 Task 1, focusing on **Hate Speech Identification**. The project includes datasets for training and testing, a Jupyter notebook for the logits ensemble, and a model directory for future model implementation.

## Project Structure

The repository contains the following main directories and files:

```
BLP25-Task1/
│
├── Dataset/
│   ├── Train Set/
│   │   ├── subtask_1A/
│   │   ├── subtask_1B/
│   │   ├── subtask_1C/
│   │
│   ├── Test Set/
│       ├── blp25_hatespeech_subtask_1A_test.tsv
│       ├── blp25_hatespeech_subtask_1B_test.tsv
│       ├── blp25_hatespeech_subtask_1C_test.tsv
│
├── Logits Ensemble/
│   ├── Logits Ensemble.ipynb
│
└── Model/
    ├── Hate Severity
    ├── Hate Type
    ├── To Whom
```

## Dataset

### Train Set
The **Train Set** contains the following subtask datasets:
- **subtask_1A**: Dataset for classifying hate speech type
- **subtask_1B**: Dataset for identifying the target of hate speech
- **subtask_1C**: Dataset for classifying hate speech based on its type, severity, and target

### Test Set
The **Test Set** contains the following files:
- **blp25_hatespeech_subtask_1A_test.tsv**: Test data for subtask 1A
- **blp25_hatespeech_subtask_1B_test.tsv**: Test data for subtask 1B
- **blp25_hatespeech_subtask_1C_test.tsv**: Test data for subtask 1C

## Logits Ensemble

The **Logits Ensemble** directory contains a Jupyter notebook titled `Logits Ensemble.ipynb`, which provides the code for the logits ensemble approach for combining different model predictions.

## Model

The **Model** directory contains the following files:
- **Hate Severity**
- **Hate Type**
- **To Whom**

These files are intended for use in implementing machine learning models. You can add your own models or modify these files as needed.

## Setup

To get started, you need to have the following dependencies:

- Python 3.x
- Jupyter Notebook (for running `Logits Ensemble.ipynb`)
- Required libraries: `pandas`, `numpy`, `sklearn`, `tensorflow`, etc.

You can install the required libraries using `pip`:

```bash
pip install -r requirements.txt
```

## Usage

1. Clone the repository:

```bash
git clone <repo_url>
cd BLP25-Task1
```

2. Run the Jupyter notebook for logits ensemble:

```bash
jupyter notebook Logits Ensemble/Logits Ensemble.ipynb
```

3. Add your models to the **Model** directory and train them using the provided dataset.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
