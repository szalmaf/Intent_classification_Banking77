Transforming intent
===================


This notebook aims to show a performance comparison of three natural language models: our baseline, the **Naive Bayes model**, a pre-trained and then fine-tuned **DistilBert** model from HuggingFace and **Google**'s conversation engine, **Dialogflow**.

The three models are trained on the same dataset, the **Banking77 dataset** from ... with roughly 13,000 utterance-intent pairs. There are 77 different labels as the dataset's name suggests, so the sample size per class is roughly 170 per class. 


### Basic stats of dataset

#### Intent distribution

The intent histogram below shows that the **intent distribution** is relatively **balanced**. The largest unbalance between *contactless_not_working* and *virtual_card_not_working* vs. *card_payment_fee_charched* is a factor of three but overall this data set is more balanced than what one typically experiences in real life. Even the least frequent intents occur 75 times.
