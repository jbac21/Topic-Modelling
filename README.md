# Topic-Modelling

Non Negative Matrix Factorization (NMF) and Latent Dirichlet Allocation (LDA) are often used for topic modelling. While most blogs explain how they can be applied using the Gensim or scikit-learn library, less is known about the optimization of these models.

The proposed code uses the scikit-learn pipeline to connect classes for data preprocessing, data transformation and topic modelling. The order of the classes is aligned to the Knowledge Discovery in Databases Framework (Fayyad et al. 1996). The implementation uses popular frameworks for data preprocessing and uses scikit-learn wrappers (custom transformers and custom estimators) to wrap these classes to the scikit-learn API. The gensim coherence model is integrated into a GridSearch class and used to evaluate the topic composition. 

How to optimize these models?
- 

![image](https://user-images.githubusercontent.com/77205454/126347577-f20ad3a5-4075-4266-9782-7947baf3e03f.png)
