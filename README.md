# Credit_Risk_Analysis


## Overview of the analysis:
The purpose of this analysis is to use imbalanced data Machine Learning methods to predict high risk credit cards. 

## Results: 
- Recall is the ability of the classifier to find all the positive samples, whereas Precision is the measure of how reliable positive classifications are. 
- As expected, our precision for low-risk credit cards was 1 for all of the models. This is because credit card data is a classic example of imbalanced data, where the vast majority of credit card applicants are low-risk. 
- Our ensemble classifiers (Balanced Random Forest and AdaBoost) produced the highest precision scores for high-risk cards at 3% and 9%, respectively. This means that there are a high amount of false positives.
- Overall, the AdaBoost Classifier was the best because it had the highest precision for high-risk applicants, but also had the highest sensitivity (meaning it captured all credit cards that were potentially high risk -- 92%). 

**1. Naive Random Oversampling**<br>
<img width="788" alt="Screen Shot 2021-10-26 at 8 24 17 PM" src="https://user-images.githubusercontent.com/10199828/138979587-06598a23-a819-4611-a719-d3734a9233f1.png">
<br>
**2. SMOTE Oversampling** <br>
<img width="769" alt="Screen Shot 2021-10-26 at 8 24 57 PM" src="https://user-images.githubusercontent.com/10199828/138979657-fde4a002-f122-47a5-b533-9a887bb52193.png">
<br>
**3. Undersampling via Cluster Centroids**<br>
<img width="780" alt="Screen Shot 2021-10-26 at 8 25 34 PM" src="https://user-images.githubusercontent.com/10199828/138979710-fad665e6-d65a-4e4d-8d23-8255b6c7bbe3.png">
<br>
**4. SMOTEEN Undersampling and Oversampling**<br>
<img width="791" alt="Screen Shot 2021-10-26 at 8 26 06 PM" src="https://user-images.githubusercontent.com/10199828/138979750-a28ce795-bfce-4e48-88b9-f253c5555907.png">
<br>
**5. Ensemble: Balanced Random Forest Classifier**<br>
<img width="780" alt="Screen Shot 2021-10-26 at 8 26 49 PM" src="https://user-images.githubusercontent.com/10199828/138979798-afbb50dc-561a-4019-9020-a57f43fb3b03.png">
<br>
**6. Ensemble: Easy Ensemble AdaBoost Classifier**<br>
<img width="782" alt="Screen Shot 2021-10-26 at 8 27 28 PM" src="https://user-images.githubusercontent.com/10199828/138979839-50dec56c-0581-487d-a190-1bfb3ee22632.png">
<br>

## Summary: 
In summary, I would recommend using the AdaBoost Ensemble Classifier. Across the models, it has the highest F1 score. While the model suffers from low precision (9%), it makes up for through it's high sensitivity. The model's recall is 92%, which means that it has relatively few false negatives and does a good job of making sure no bad credit card applicants slip by. 

That being said, it might be useful looking at other types of ensemble classifiers considering both AdaBoost and Balanced Random Forest produced the most best results. 


