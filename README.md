# Topic-Modelling

Non Negative Matrix Factorization (NMF) and Latent Dirichlet Allocation (LDA) are often used for topic modelling. While most blogs explain how they can be applied using the Gensim or scikit-learn library, less is known about the optimization of these models.

The proposed code uses the scikit-learn pipeline to connect classes for data preprocessing, data transformation and topic modelling. The order of the classes is aligned to the Knowledge Discovery in Databases Framework (Fayyad et al. 1996). The implementation uses popular frameworks for data preprocessing and uses scikit-learn wrappers (custom transformers and custom estimators) to wrap these classes to the scikit-learn API. The gensim coherence model is integrated into a GridSearch class and used to evaluate the topic composition. 

### How to optimize models?
- Pass hyperparameter values as model_params. State the class first, then behind __ denote the parameter for optimization and a list of values (s. image below)
- Classes for preprocessing and transformation can be commented out to be excluded from the model.
- There are two empty lists for named entity removal and stop word removal. Both can be customized to remove additional words from the corpus.
- All coherence scores and hyperparameter values are listed by GridSearch and can be saved as csv. The model having returned the best coherence score can be identified by sorting the list of values for an evaluation metric.

![image](https://user-images.githubusercontent.com/77205454/126347577-f20ad3a5-4075-4266-9782-7947baf3e03f.png)

### How to eyeball the results?
- Single models can be estimated and their topic composition can be printed.
- pyLDAvis has been added for LDA.
