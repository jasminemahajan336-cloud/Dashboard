# Dashboard
# NLP Explorer — Interactive NLP Pipeline Analyzer

NLP Explorer is an interactive Natural Language Processing (NLP) dashboard built with Python. It provides a simple interface for entering text and exploring several NLP operations through tables, charts, and visualizations.

## Features

- **Tokenization** — Displays the individual tokens extracted from the input text.
- **POS Tagging** — Shows coarse and fine-grained Part-of-Speech tags.
- **POS Distribution** — Displays the frequency of POS categories using an interactive Plotly chart.
- **Named Entity Recognition (NER)** — Identifies and visualizes named entities using spaCy.
- **Lemmatization** — Displays the lemma/base form of each token.
- **Stemming** — Applies the NLTK Porter Stemmer to the input tokens.
- **Morphology** — Displays POS and morphological information for tokens.
- **Dependency Parsing** — Visualizes syntactic dependency relationships.
- **Text Statistics** — Shows token, word, sentence, entity, stopword, and punctuation counts.

## Technologies Used

- Python 3
- spaCy
- NLTK
- Dash
- JupyterDash
- Dash Bootstrap Components
- Pandas
- Plotly

## Installation

Install the required packages:

```bash
pip install streamlit spacy nltk plotly
pip install dash jupyter-dash
pip install dash-bootstrap-components
```

Download the spaCy English language model:

```bash
python -m spacy download en_core_web_sm
```

> **Note:** The notebook currently installs both Streamlit and Dash/JupyterDash, but the dashboard itself is implemented using Dash/JupyterDash.

## How to Run

1. Clone or download this repository.
2. Open `dashboard.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab.
3. Install the required dependencies.
4. Download the `en_core_web_sm` spaCy model.
5. Run the notebook cells.
6. Enter or paste text into the input box.
7. Click **Analyze Text**.
8. Explore the results using the available tabs.

The dashboard is configured to run inline in a Jupyter environment.

## Dashboard Tabs

| Tab | Description |
|---|---|
| Overview | Displays a summary of the text analysis |
| Tokens | Lists all tokens |
| POS Tagging | Displays POS and fine-grained tags |
| POS Distribution | Shows POS frequency as a bar chart |
| NER | Visualizes recognized named entities |
| Lemmatization | Displays token and lemma pairs |
| Stemming | Displays token and Porter stem pairs |
| Morphology | Displays token, POS, and morphology |
| Dependencies | Visualizes dependency relationships |

## NLP Pipeline

```text
User Input
    ↓
spaCy NLP Processing
    ↓
Tokenization
    ├── POS Tagging
    ├── Named Entity Recognition
    ├── Lemmatization
    ├── Morphological Analysis
    └── Dependency Parsing
    ↓
NLTK Porter Stemmer
    ↓
Interactive Dashboard
```

## Example Input

The notebook contains the following example text:

```text
On Monday, September 15, 2025, at 10:00 AM EST, Dr. Helena Vance
announced that the company's new AI research lab in San Francisco
would open next quarter, aiming to hire over 200 engineers.
```

You can replace this with your own English text.

## Project Structure

```text
NLP-Explorer/
│
├── dashboard.ipynb
└── README.md
```

## Project Objective

The project was developed to provide an interactive interface for performing and understanding common NLP operations, including:

1. Named-Entity Recognition
2. POS Tagging
3. POS Distribution
4. Lemmatization
5. Stemming
6. Morphology
7. Dependencies

## Notes

- The project uses spaCy's `en_core_web_sm` model for English NLP processing.
- NLTK's `PorterStemmer` is used for stemming.
- The dashboard uses Bootstrap components for its interface.
- Plotly is used for the POS distribution visualization.
- The notebook uses `JupyterDash` and is configured for inline execution.

## License

This project is intended for educational and academic purposes.
