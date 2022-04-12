# NLP-Toxic-comment-classification

This is the repository for the NLP project in the context of IASD and MASH masters, PSL university : toxic comment classification. The dataset, found on Kaggle, is made of comments, classified into classes : toxic, severe toxic, obscene, threat, insult, identity_hate and regular comments.

In this work, we tested several methods : 
- Apply a Bag Of Words (BOW) + Logistic Regression classifier
- Use GPT2 to obtain embeddings from words in the comments, that we stack in a padded matrix. Then, apply a MLP or a RandomForest on this matrix
- Extend the Multi-Level Graph Neural Network (slightly modified) to a multi-class text classification, on large sentences.

The notebook Dataset_stats.ipynb contains several statistics per class (average comment length per class, average number of ! per comment per class). 
The notebook BOW.ipynb illustrates a Bag Of Words + Logistic Regression classifier on the dataset.
The notebook MLP&RandomForest.ipynb uses a MLP and a RandomForest on a matrix obtained with GPT2 embeddings.
Finally, the MLGNN.ipynb extends the MLGNN framework to our multi-class text classification problem, with long sentences.

The pdf file report.pdf analyzes our work. 

