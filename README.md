# Introduction and Goal of the Study
Document classification, a subfield of NLP, is the process of predicting group membership for data instances, meaning organizing documents into predefined categories or classes based on their content. The main objective of this study is to introduce and evaluate a selection of promising Free Open-Source Software (FOSS) approaches for document classification and compare them against each other regarding their prediction performance and efficiency to identify the best candidate for a specific use case. In addition, the study compares the selected approach’s prediction performance, efficiency, and cost-effectiveness with commercial providers’ proprietary software. This comparison can provide insights into different approaches’ relative strengths and weaknesses to help businesses decide on the best strategy for their needs. However, it is essential to note that this thesis focuses solely on a specific use case, and therefore, the results presented may not be generalizable to other use cases.

# Dataset

In the context of many businesses, the distinctions between different categories can be subtle, and the textual content may be intended for a specific, targeted audience rather than a general audience. For this reason, this thesis focuses on the [Consumer Complaint Database](https://www.consumerfinance.gov/data-research/consumer-complaints/) from the Consumer Financial Protection Bureau (CFPB). This U.S. government agency collects consumer complaints through formal, textual exchanges between companies, public institutions, and private individuals. This dataset represents a scenario similar to how private individuals typically communicate with businesses and therefore provides a relevant and applicable context for the study of document classification. The dataset comprises 3,218,032 consumer complaints. The focus will be on the textual content provided in the Consumer complaint narrative and the class provided by the Product column.

# Methodology

The study involved comparing various FOSS machine learning software against proprietary software offered by commercial providers. Several FOSS models were initially researched, including traditional statistic-based methods such as Naive Bayes Classifiers (NBCs), K-Nearest Neighbors (KNN) algorithms, decision tree classifiers, logistic regression, and Support Vector Machines (SVMs). Next, deep learning approaches, including Long Short-Term Memory (LSTMs), Bidirectional LSTMs (Bi-LSTMs), Gated Recurrent Units (GRUs), Convolutional Neural Networks (CNNs), and Pretrained Language Models (PLMs) such as BERT, RoBERTa, XLNet, and GPT-2 were examined. Finally the best-performing FOSS approach was compared again the following commercial prodcuts: Microsoft Azure, Amazon Comprehend, OpenAI’s GPT-3,  Levity AI, Planet AI, Google Vertex AI. This comparison was achieved by training each model on the same training dataset and inferring on the same test dataset.

# Comparison of Approaches

The best-performing FOSS model, as determined by the evaluation metrics, specifically the accuracy, was then pitted against the proprietary software to determine how it compares. The comparison process entailed assessing three principal costs associated with the products, specifically training costs, hosting costs, and inference costs, which constitute the total pricing of the products in most cases. This thesis simulates a 30-day period, during which the classification model will be trained on the first day, hosted for the entire duration, and inference costs computed for varying document volumes. 

# Results

The results obtained in this study may be specific to the datasetand use case considered in this study. Therefore, different datasets and use cases may produce different results, and it is essential to evaluate the models on the specific use case to determine the most suitable model.

## FOSS Performance:

![alt text](https://github.com/LeonGoergen/DocumentClassification/blob/main/assets/foss.png)

## Proprietary Results:

![alt text](https://github.com/LeonGoergen/DocumentClassification/blob/main/assets/prop.png)

## Cost-Comparison:

![alt text](https://github.com/LeonGoergen/DocumentClassification/blob/main/assets/costs.png)
