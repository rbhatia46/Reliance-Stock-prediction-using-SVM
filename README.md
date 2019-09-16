# SVM for predicting buy/sell of Reliance Stock
Comparing different SVM Kernels, specifically the linear kernel, polynomial kernel, and the Radial Basis Function Kernel, in their effectiveness when applied to predict buy/sell of Reliance Stock. A much detailed approach can be found on the accompanying [Medium article](https://medium.com/@e22aafa7d95/abb494d9f45f)
## Model details
Featuresets: various technical indicators for Reliance Stock
Labels: - Buy/Sell
	- Buy - if price is predicted to rise 
	- Sell - of price is predicted to drop

### Results (Accuracy)
- Linear kernel: 51.43%
- Polynomial Kernel: 53.15%
- Radial Basis Function Kernel: 52.00%
- Random Model Accuracy : 33%	

### Interesting aspects for improvement:
- Effects of feature standardization on SVMs
- Predictability of certain technical indicators, can be studied using Hypothesis Testing
- Use Sentiment Analysis and news on Reliance Stock/Stocks in your portfolio.
- Use more number of technical indicators(since SVM works well with high-dimensional data, you can easily add more features without worrying much about the curse of dimensionality).
- Apply the same on a diversified portfolio of stocks rather than a single stock.
- Find a domain-specific kernel, which can give the performance a significant boost, i.e., a kernel which works well for finance/time-series data, this needs some research.
- Fine-tune the existing SVM Architecture (use RandomSearch rather than GridSearch to make life easier)
- Interpret your model with model agnostic techniques (such as LIME)to understand any bias(if it exists) and understand which feature is contributing more to your prediction.
- Use more data(even more than 10 years of data) to obtain much better results, which of course comes at the cost of more time required to train the SVM.
- Try other classifiers, such as KNN, which can be quite similar to RBF-based SVM to see if there is any improvement in the performance.
