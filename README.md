# Neural-Network-and-AI

In this report, “Sentiment Analysis on Reddit Comments using Different Neural Networks”, it is proposed the implementation and evaluation of different single and hybrid CNN and RNN models for sentiment analysis (classification). Some reference models are implemented and compared against a new (proposed) model.

The Introduction section discusses the importance of sentiment analysis with an emphasis on social network data and applications. The main goal and the research questions are clearly described. The methodological approach, which consists of i) replicating some proposed models from the literature, and ii) propose and evaluate a new model, based on the reference models, is also described. A summary of the main findings is presented in the Abstract.

The solution concept is based on reference models from the literature which have informed the design of a bespoke model. The reference models (D-CNN, Bidirectional LSTM and a hybrid Bidirectional LSTM + CNN) were replicated to assess the reported performance but using a slightly bigger dataset (compared to those used in the papers). The D-CNN is designed to handle long-term semantic features (as reported) and was slightly modified in this work to accommodate different dilation configurations. A CNN model is also used for comparison purposes. A bidirectional LSTM is further defined and compared against a standard LSTM model. Finally, a hybrid bidirectional LSTM + CNN model is defined and tested. A bespoke model based on dilated CNN and bidirectional LSTM is then proposed. Some strategies to avoid overfitting are explored (early stopping, dropout and L2 regularization). All models were assessed through standard metrics. 

The implementation involved building CNN, LSTM and their hybrid models using Keras. Then all these models with different embedding layers are considered (Word2vec versus Glove). T

The dataset used comprises 37,000 comments on the 2019 General Elections in India held in the Reddit service. Some important characteristics of the dataset are commented, as the colloquial writing style, character length limit, and controversial contexts of some words. Data is labelled as 1 and -1 for positive and negative comments, with a huge class imbalance. A total of 16,000 comments were equally sampled from both classes, and training and testing samples were created. 

The numerical evaluation involved plotting train/test loss and accuracy curves for different models and comparing their performance via several standard metrics. Th

The Conclusion section draws on the superior performance of the proposed model over the existing models adapted from the literature. 
