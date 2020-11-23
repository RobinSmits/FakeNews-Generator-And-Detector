# FakeNews-Generator-And-Detector

Recently I was experimenting with the T5 model and exploring the options it has to offer. Thinking about the Summarization capabilities of current State-of-the-Art NLP models I was curious to find out what the result could be if I would turn that around. So input a short text and let the model generate a longer text. If I would also use a News dataset for that than I would have a very simple Fake News generator. Next I could use that real and fake news to train a classifier and see how well yet another NLP model would be able to classify the real and fake news.

To summarize this repository contains the code for the following 3 steps:
- Train a T5 model on a news dataset and generate a full set with fake news.
- Train a RoBERTA model to be able to classify the real and fake news.
- With an unseen test set first generate fake news with the T5 model and then have the RoBERTa model classify the real and fake news.

As news dataset I used the Tensorflow Datasets ['ag_news_subset'](https://www.tensorflow.org/datasets/catalog/ag_news_subset). It is primarily used for news topic classification but since it contains a 'title' and longer 'description' for 120K news articles it is perfect to use for my fake news generator and detector.

<< To Do .. Finalize >>