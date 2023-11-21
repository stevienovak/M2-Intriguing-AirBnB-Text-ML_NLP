# M2-Intriguing-AirBnB-Text-ML_NLP

- **Supervised Learning** - Leveraging traditional Machine Learning models to transform customer review text into insightful classification predictions. 
- **Supervised Learning** - NLP BERT & Distilled-BERT to build a sentiment prediction model, decoding customer sentiment with 97.6% accuracy
- **Unsupervised Learning** - LDA and NMF model to identify and categorize customer feedback
  

## Introduction

In this sharing economy where online reviews lack anonymity, the act of contributing a negative review amidst a sea of positive ones may amplify psychological discomfort. This stems from an inherent sense of divergence perceived by the author in relation to  the opinions of the majority (J.Meijerink, E.Schoenmakers, 2019). From customers’ perspective, considering the hosts’ autonomy to reject potential guests, it becomes imperative for guests to accumulate favorable reviews as much as the hosts themselves. Thus the stakes are high on both sides as reputation hangs on a balance. Given the unique behavioral idiosyncratic traits observed within the sharing economy, it was discovered that for Airbnb, 95% of properties have an average rating of 4.5 to 5 stars. Virtually no property has 3.5 stars and below  as compared to tripadvisor,  which has more variance in the reviews and has an average rating of 3.5 stars (Georgios. Z et al., 2018). From a guest perspective, discerning the distinction between ratings such as 4.7 and 4.8 can prove challenging. Alison.P, 2020 mentioned in an article written for the WallStreet Journal (“WSJ”) that beyond reliance on the star ratings, consumers should scrutinize the content of reviews as there may be subtle messages unveiled about the quality of the property. Descriptions may allude to potential red flag issues eluding the high rating given. 

Findings from past research papers underscore the potential opportunity to investigate questions regarding consumers’ reviews, specifically analyzing whether these reviews can provide a more precise and contextualized measure of a guest's unique experience with an Airbnb listing. To achieve this, we will employ a methodology involving the extraction of sentiments from consumer reviews, their subsequent normalization, and classification within the range of 0 to 4 (0 representing the lowest and 4 the highest). Our goal is to construct a machine learning sentiment scoring model capable of predicting and assessing each property’s rating based on the text reviews received. This process promises to yield a more nuanced evaluation tool within the sharing economy, enhancing the precision of property appraisals. 

Once this model is operational, we foresee that hosts would benefit significantly from a more insightful understanding of customer feedback. To achieve this, we propose to implement unsupervised learning in the form of topic modeling on Airbnb reviews. The aim is to uncover prevalent themes within guests' feedback, offering valuable insights into the focal points of guests' concerns. This knowledge will empower Airbnb hosts to address specific areas of concern and effectively meet their guests' expectations, thereby optimizing the user experience on the platform. 

## Summary of key findings for supervised and unsupervised learning

_`Finding for supervised learning`_ : Through the supervised learning work, we encountered instances where despite high traditional rating scores, underlying issues were discernible within the review text. Our model successfully identified these negative sentiments, recalibrating the review score based on the text itself to provide a more accurate reflection of the guest experience. This underlines the model's capacity to capture nuanced feedback often overlooked by conventional rating systems, thereby delivering a more comprehensive and authentic appraisal of the property quality.

_`Finding for unsupervised learning`_ : Through the application of unsupervised learning, we discovered prevalent themes that arise within guest feedback and the analysis exposed key areas of guest concern, shedding light on aspects that significantly impact their experiences. Capability of the model to identify and categorize customer feedback into actionable themes underscores its potential as a vital tool for hosts. It empowers hosts with the insights necessary to address specific areas of concern, allowing them to align their offerings more accurately with guest expectations. 

## Key Highlights ##

### Supervised Learning, NLP - Model Training, Text Prediction ### 
Performance outcomes of BERT and Distilled-BERT significantly exceeded expectations. F1_Macro and accuracy scores at 0.942 and 0.937 notably outstripped those of conventional machine learning models. 



<a href="URL_REDIRECT" target="blank"><img align="center" src="https://raw.githubusercontent.com/stevienovak/inventories/main/Bert_classification_table.jpg" height="300" /></a>
Figure 1: BERT and Distilled BERT Confusion Matrix

<a href="URL_REDIRECT" target="blank"><img align="center" src="https://raw.githubusercontent.com/stevienovak/inventories/main/F1_accuracy_precision_table.jpg" height="160" /></a>
Figure 2: BERT Classification Report

We tested the distilled BERT model with new data and the model demonstrated strong performance, underscoring its efficacy in dealing with new data. 

<a href="URL_REDIRECT" target="blank"><img align="center" src="https://raw.githubusercontent.com/stevienovak/inventories/main/Prediction_sample.jpg" height="200" /></a>
Figure 3: Prediction Test on New Data

BERT and Distilled-BERT demonstrated a superior performance in handling these nuanced sentiment categorizations, thereby yielding better results. This signifies the promise of deep learning models in effectively capturing the intricate nature of human sentiments, which may be a valuable direction for future research. 

### Unsupervised Learning, LDA, NMF ### 

Based on best performance model - LDA, topic modeling using gensim on negative sentiment sub-dataset showed keywords such as ‘dirty’. ‘Towel’, ‘clean’, ‘bed’, ‘bathroom’, ‘toilet’, ‘cleaning’, ‘floor’, ‘sheet’, ‘hair’, ‘shower’ which seem to highlight cleanliness issues! Topic can be labeled as ‘Cleanliness Is Key’ or ‘Banish Bathroom / Bedroom Blunders’. Positive sentiment sub-dataset showed keywords such as ‘clean’, ‘host’, ‘location’, ‘recommend’, ‘comfortable’, ‘easy’, ‘responsive’, ‘area’, ‘space’, ‘quiet’, ‘close’ which we interpreted as key traits which makes one accommodation stand out from another. We can label this topic as “Responsive Host with Clean Quiet Convenient Space”. 

<a href="URL_REDIRECT" target="blank"><img align="center" src="https://raw.githubusercontent.com/stevienovak/inventories/main/LDA_Neg_Sen.jpg" height="400" /></a>
Figure 4: Top 30 Topics vs Nearest Distance - Neg

<a href="URL_REDIRECT" target="blank"><img align="center" src="https://raw.githubusercontent.com/stevienovak/inventories/main/LDA_Pos_Sen.jpg" height="400" /></a>
Figure 5: Top 30 Topics vs Nearest Distance - Pos

## Reference
Meijerink J, Schoenmakers E. (2019).  Why are online reviews in the sharing economy skewed toward positive ratings? Linking customer perceptions of service quality to leaving a review of an Airbnb stay. Retrieved May 27, 2023 from https://www.researchgate.net/publication/340538870_Why_are_online_reviews_in_the_sharing_economy_skewed_toward_positive_ratings_Linking_customer_perceptions_of_service_quality_to_leaving_a_review_of_an_Airbnb_stay 

Georgios. Z, Proserpio. D, Byers J. (2020). A First Look at Online Reputation on Airbnb, Where Every Stay is Above Average. Retrieved May 27, 2023 from https://people.bu.edu/zg/publications/airbnbreviews.pdf

Pohle, A. (2023). Four Stars for Peeling Paint and Broken Doors? What’s Behind High Airbnb Ratings. Retrieved May 27, 2023 from https://www.wsj.com/articles/four-stars-for-peeling-paint-and-broken-doors-whats- behind -high-airbnb- ratings-da26390e

Karl H., Victor C., Chrisina J. (2022). A review on Natural Language Processing Models for COVID-19 research. Retrieved Jun, 15, 2023 from https://www.sciencedirect.com/science/article/pii/S2772442522000326

Veerle V, Louise C, Matthew W, Libby B, Laurence H. (2011). Managing and Sharing Data, Best Practice for Practitioners. Retrieved Jun, 16, 2023 from https://dam.ukdataservice.ac.uk/media/622417/managingsharing.pdf 
