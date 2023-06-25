# M2-Intriguing-AirBnB-Text-ML_NLP
Using NLP - BERT to build a sentiment prediction model
In this sharing economy where online reviews lack anonymity, the act of contributing a negative review amidst a sea of positive ones may amplify psychological discomfort. This stems from an inherent sense of divergence perceived by the author in relation to  the opinions of the majority (J.Meijerink, E.Schoenmakers, 2019). From customers’ perspective, considering the hosts’ autonomy to reject potential guests, it becomes imperative for guests to accumulate favorable reviews as much as the hosts themselves. Thus the stakes are high on both sides as reputation hangs on a balance. Given the unique behavioral idiosyncratic traits observed within the sharing economy, it was discovered that for Airbnb, 95% of properties have an average rating of 4.5 to 5 stars. Virtually no property has 3.5 stars and below  as compared to tripadvisor,  which has more variance in the reviews and has an average rating of 3.5 stars (Georgios. Z et al., 2018). From a guest perspective, discerning the distinction between ratings such as 4.7 and 4.8 can prove challenging. Alison.P, 2020 mentioned in an article written for the WallStreet Journal (“WSJ”) that beyond reliance on the star ratings, consumers should scrutinize the content of reviews as there may be subtle messages unveiled about the quality of the property. Descriptions may allude to potential red flag issues eluding the high rating given. 
Findings from past research papers underscore the potential opportunity to investigate questions regarding consumers’ reviews, specifically analyzing whether these reviews can provide a more precise and contextualized measure of a guest's unique experience with an Airbnb listing. To achieve this, we will employ a methodology involving the extraction of sentiments from consumer reviews, their subsequent normalization, and classification within the range of 0 to 4 (0 representing the lowest and 4 the highest). Our goal is to construct a machine learning sentiment scoring model capable of predicting and assessing each property’s rating based on the text reviews received. This process promises to yield a more nuanced evaluation tool within the sharing economy, enhancing the precision of property appraisals. Once this model is operational, we foresee that hosts would benefit significantly from a more insightful understanding of customer feedback. To achieve this, we propose to implement unsupervised learning in the form of topic modeling on Airbnb reviews. The aim is to uncover prevalent themes within guests' feedback, offering valuable insights into the focal points of guests' concerns. This knowledge will empower Airbnb hosts to address specific areas of concern and effectively meet their guests' expectations, thereby optimizing the user experience on the platform. 
Summary of key findings for supervised and unsupervised learning 
Finding for supervised learning: Through the supervised learning work, we encountered instances where despite high traditional rating scores, underlying issues were discernible within the review text. Our model successfully identified these negative sentiments, recalibrating the review score based on the text itself to provide a more accurate reflection of the guest experience. This underlines the model's capacity to capture nuanced feedback often overlooked by conventional rating systems, thereby delivering a more comprehensive and authentic appraisal of the property quality.
Finding for unsupervised learning: Through the application of unsupervised learning, we discovered prevalent themes that arise within guest feedback and the analysis exposed key areas of guest concern, shedding light on aspects that significantly impact their experiences. Capability of the model to identify and categorize customer feedback into actionable themes underscores its potential as a vital tool for hosts. It empowers hosts with the insights necessary to address specific areas of concern, allowing them to align their offerings more accurately with guest expectations. 