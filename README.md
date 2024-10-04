# MsDS-unsupervised-nlp-sfdc-classification

**DTSA 5510 Unsupervised Algorithms in Machine Learning**

## Abstract
This project explores the application of unsupervised learning models to categorize large volumes of Salesforce help documentation. Salesforce, like many software companies, produces extensive documentation, which can be challenging to organize into categories. Using Natural Language Processing (NLP), features from 1,498 documents across Salesforce’s Service Cloud and Sales Cloud were extracted to identify clusters and relationships in the text.

The data was collected using a web scraping tool, and the dataset was labeled into 11 categories, representing the hierarchical structure of Salesforce documentation. These labels were used to assess the accuracy of two unsupervised learning models: KMeans clustering and Non-Negative Matrix Factorization (NMF). The dataset was split into 80% for training, 10% for validation, and 10% for final testing.

The objective was to develop models that replicate Salesforce’s clustering of content based purely on textual patterns. The models would enable the automatic categorization of new documents and streamline the labeling of unseen articles. Both KMeans and NMF models were developed, with hyperparameter tuning applied to improve performance. Final evaluations were conducted using accuracy as the key metric.

The notebook covers several stages of analysis: data exploration, feature engineering, model development, and tuning. Ultimately, the project demonstrates the effectiveness of unsupervised learning techniques in document clustering and offers insights for automating content organization.


## Conclusion

**KMeans Cluster Model Results:**

The KMeans clustering model achieved a training accuracy of 49.5% and a validation accuracy of 53.0%. While these results indicate some ability of the model to group similar documents, the relatively moderate accuracy suggests that further optimization or alternate clustering approaches could improve performance.

**NMF (Non-Negative Matrix Factorization) Baseline Model Results:**

The baseline NMF model performed better than KMeans, achieving a training accuracy of 56.4% and a validation accuracy of 62.6%. This indicates that NMF was more effective at identifying latent patterns in the text data, but there was still room for improvement.

**NMF (Non-Negative Matrix Factorization) Final Model Results:**

After hyperparameter tuning, the final NMF model showed significant improvement with a training accuracy of 64.6%, a validation accuracy of 62.6%, and a testing accuracy of 62.6%. These results demonstrate that the final NMF model was able to capture more relevant features in the data and provide more accurate clustering compared to the initial models. 
