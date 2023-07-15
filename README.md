# Capstone on Machine Learning using Python

## _Predicting Fraud Detection_

[![Image from Gyazo](https://i.gyazo.com/255db1fa2d463278e010c0527dd9bb5d.png)](https://gyazo.com/255db1fa2d463278e010c0527dd9bb5d)
[![Image from Gyazo](https://i.gyazo.com/46cbd180adcca54be21cc4236e70d3cf.png)](https://gyazo.com/46cbd180adcca54be21cc4236e70d3cf)

#

#### Description of Dataset

The dataset describes the transactions of money using a simulator to generate synthetic data based on 1 month of original financial logs from a company in Africa. The dataset has a size of 6,353,307 rows.

#### General Observations
* There are no transactions to merchants for fraud while non fraud has transactions for both merchants and customers.
* For fraud and non fraud transactions, the origin accounts are unique and have no duplicates found in destination accounts.
* Transactions for transfer and cash out are done within the hour for fraud.
* Same amounts transacted for transfer and cash out could be fraud or non fraud. However, the duration of transactions determine its fraudulent nature.
  * For example, for non fraud, difference between transactions are negative whereas fraud is almost always a positive difference.
* Overall, fraud behaviour is determined by the same amount transacted for transfer and cashout and the transactions have to happen within the hour.
* For ML models, accuracies of both models are reduced at 80% training data as compared to at 50% training data

#### Insights
* Easier to predict as the data is well balanced, clean and clear cut
* Model could also be biased so will need more data as input to better train the model
* Having a split of more training data does not always result in better accuracies due to overfitting. Similarly, too little of training data may result in underfitting.
  * Number of iterations also play apart in the accuracy of model.
* Does not accurately reflect actual fraudsters as it is evident that based on the dataset transactions of same amounts happen within the same hour. Hence, if this happens in real life, it is easily detected as fraud.


#### Other Comments
As the dataset filtered and used as input is balanced, could consider increasing the size of the clean and filtered dataset to improve both models.

As the behaviour of the data is consistent, could consider tweaking the dataset by oversampling and undersampling with insufficient data as the input data. 

#### Connect with Me!
Like my work? Send me a DM on [Linkedin!](https://sg.linkedin.com/in/noor-mustikha-nk)
