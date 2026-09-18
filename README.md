# Machine Learning Coursework

Three completed NLP and machine learning experiments, collected in one repository. Each directory contains one cleaned notebook. Notebook outputs were removed from the published copies; the figures below come from the saved local runs and have not been independently rerun for this release.

| Project | Task | Recorded test result |
| --- | --- | --- |
| [Assignment 01](assignment-01-sentiment/) | Binary bag-of-words sentiment classification with a hand-built hinge-loss linear model | 88.25% accuracy |
| [Assignment 02](assignment-02-pos-tagging/) | Baseline, LSTM, and GRU for English, Chinese, and Japanese POS tagging | LSTM: 87.97%, 84.59%, 91.30% token accuracy |
| [Assignment 03](assignment-03-transformers/) | IMDb sentiment classification with BERT, DistilBERT, mBERT, logistic regression, and a random baseline | BERT: 93.22% accuracy |

## Run

Use Python 3 and Jupyter. Install the packages in `requirements.txt`, then open the notebook from its own project directory so relative data paths work. Transformer training in Assignment 03 requires substantial compute and downloads pretrained models.

The datasets and model checkpoints are **not included**. Obtain datasets from their original distributors and follow their terms:

- Assignment 01: [Cornell Review Polarity v2.0](https://www.cs.cornell.edu/people/pabo/movie-review-data/). Extract `txt_sentoken/` inside `assignment-01-sentiment/`.
- Assignment 02: [Universal Dependencies](https://universaldependencies.org/) English EWT, Chinese GSD, and Japanese GSD. The notebook downloads current repository snapshots into `assignment-02-pos-tagging/data/`; those may differ from the snapshot used for the recorded results.
- Assignment 03: [Stanford Large Movie Review Dataset](https://ai.stanford.edu/~amaas/data/sentiment/). Extract `aclImdb/` into `assignment-03-transformers/data/`.

The notebooks are coursework experiments, not packaged production models. Results from different assignments use different datasets and should not be compared as if they shared one benchmark.
