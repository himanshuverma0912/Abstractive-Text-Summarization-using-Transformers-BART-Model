## Abstractive Text Summarization using Transformers-BART Model (Overview)

This project aims to generate concise and informative summaries of text documents using the BART model. The model is trained on a dataset of text and corresponding summaries, enabling it to learn the key points and rephrase them into a shorter, human-readable format.

### BART

BART stands for Bidirectional and Auto-Regressive Transformer. Its primary features are a bidirectional encoder from BERT and an autoregressive decoder from GPT. The encoder and decoder are united using the seq2seq model to form the BART algorithm.

To understand the BART transformer, one needs to closely look at BERT and GPT. BERT performs the Masked Language Modelling with the help of its bidirectional transformer and predicts the missing values. On the other hand, GPT uses its autoregressive decoder to predict the next token in a sentence.


### Dataset
The data used is from the curation base repository, which has a collection of 40,000
professionally written summaries of news articles, with links to the articles themselves.
The data is cloned from GitHub. Then data is downloaded in the form of a CSV file
and has the following features:
• Article titles – title for the texts
• Summaries – summary for each text
• URLs – the URL links
• Dates
• Article content – content under each article

========================================================================================

<strong>The process is as follows:</strong>

1. <strong>Make a virtual environment.</strong>

Execute the following command to create the virtual environment:
```
python -m venv myenv
```
2. <strong>Activating the Virtual Environment:</strong>

Depending on the operating system, the activation command might vary:

For Windows:

```
.\myenv\Scripts\activate
```

For macOS and Linux:

```
source myenv/bin/activate
```

2. <strong>Install dependencies</strong>

`pip install -r requirements.txt`

3. <strong>To start the app, go to output folder</strong>

`cd output`

4. <strong>Start app</strong>

`python app.py`

5. <strong>Open browser and app on defined port(default: 5000)</strong>

`localhost:5000`

### About the web app
1) Paste any news article URL and click on Submit button
2) We will see the extracted content of the news article on the Left hand side and its abstractive summarization on the Right hand side.
