# BLP25-Task1: Multi-class Hate Speech Identification

This repository contains the code and dataset for the **BLP25 Task 1**, focusing on **Multi-class Hate Speech Identification**. The project includes datasets for training and testing, a Jupyter notebook for the logits ensemble, and a model directory with various approaches for future model implementation.

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
├── Model/
│   ├── Hate Severity
│   ├── Hate Type
│   ├── To Whom
│   └── Different Approaches/
│       ├── Binary_classification_with_tact.ipynb
│       ├── blp-task-1-without_tact.ipynb
│       ├── class-weighted-loss-with-tact.ipynb
│       ├── class-weighted-loss.ipynb
│       ├── focal-loss.ipynb
│       ├── neural-network-with-2-logits.ipynb
│       ├── neural-network-with-3-logits.ipynb
│       └── random-over-sampling.ipynb
│
├── Logits Ensemble/
│   ├── Logits Ensemble.ipynb
```

## Dataset

### Train Set

The **Train Set** contains the following subtask datasets:

* **subtask_1A**: Dataset for classifying hate speech type
* **subtask_1B**: Dataset for identifying the target of hate speech
* **subtask_1C**: Dataset for classifying hate speech based on its type, severity, and target

### Test Set

The **Test Set** contains the following files:

* **blp25_hatespeech_subtask_1A_test.tsv**: Test data for subtask 1A
* **blp25_hatespeech_subtask_1B_test.tsv**: Test data for subtask 1B
* **blp25_hatespeech_subtask_1C_test.tsv**: Test data for subtask 1C

## Model

The **Model** directory contains the following files:

* **Hate Severity**
* **Hate Type**
* **To Whom**

Additionally, the **Different Approaches** directory contains the following Jupyter notebooks for exploring various machine learning strategies for hate speech classification:

* **Binary_classification_with_tact.ipynb**: A binary classification approach using TACT
* **blp-task-1-without_tact.ipynb**: A version of the task without TACT
* **class-weighted-loss-with-tact.ipynb**: Implementing class-weighted loss with TACT
* **class-weighted-loss.ipynb**: Applying class-weighted loss to the task
* **focal-loss.ipynb**: Exploring focal loss for improved classification
* **neural-network-with-2-logits.ipynb**: Neural network approach with 2 logits for prediction
* **neural-network-with-3-logits.ipynb**: Neural network approach with 3 logits
* **random-over-sampling.ipynb**: Using random over-sampling to balance the dataset

These notebooks and models can be modified or extended to fit your needs.

## Logits Ensemble

The **Logits Ensemble** directory contains a Jupyter notebook titled `Logits Ensemble.ipynb`, which provides the code for the logits ensemble approach to combine different model predictions.

## Setup

To get started, you need the following dependencies:

* Python 3.x
* Jupyter Notebook (for running `Logits Ensemble.ipynb`)
* Required libraries: `pandas`, `numpy`, `sklearn`, `tensorflow`, etc.

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

2. Add your models to the **Model** directory and train them using the provided dataset.

3. Explore the **Different Approaches** directory for various classification techniques and adapt them to improve model performance.

4. Run the Jupyter notebook for logits ensemble:

```bash
jupyter notebook Logits Ensemble/Logits Ensemble.ipynb
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
