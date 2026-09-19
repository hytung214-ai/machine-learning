# Transformer Sentiment Comparison

IMDb review sentiment experiment comparing BERT, DistilBERT, mBERT, TF-IDF plus logistic regression, and a random baseline. The recorded test accuracies are in the five `*_results.json` files; BERT reached 93.22%.

Get the [Stanford Large Movie Review Dataset](https://ai.stanford.edu/~amaas/data/sentiment/) and extract `aclImdb/` to `data/` in this directory. Run `notebook.ipynb` from here. Training checkpoints and review text are not included. Transformer training downloads pretrained models and may require a GPU.
