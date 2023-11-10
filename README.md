# Data-Bias
The goal of this assignment was to explore the concept of bias through querying the Perspective API released by Google Jigsaw. For this project, I created a dataset with comments that I made up and found online. Unfortunately, this means that for this project I used a rather small dataset and if I were to do this again I would want to use a much larger dataset.


For my hypothesis, I predicted that the uncapitalized toxic sentences will have a higher toxicity score than both the capitalized toxic sentences. From my accuracy results it seems that my hypothesis was not correct. Class 1 (i.e, > 0.5) accuracy for capitalized words/sentences was 0.67. Class 0 (i.e, < 0.5) accuracy for capitalized words/sentences was 1.0. Class 1 (i.e, > 0.5) accuracy for non-capitalized words/sentences was 0.92. Class 0 (i.e, < 0.5) accuracy for non-capitalized words/sentences was 1.0. We can see that the model was always accurate when predicting if text is toxic when the text was both capitalized and non-capitalized. So, whether the text is capitalized or not does not seem to affect the accuracy or fairness of the API. 


I think the reason my accuracy results are so uneven is because there is a significant imbalance in the number of capitalized and not capitalized sentences. This is because I was able to find more capitalized sentences online rather than not capitalized sentences. I also think I was able to get 100 percent accuracy for some of the results and very low accuracy results for others because I used such a small dataset. Using a small dataset can lead to very unreliable and skewed results which is a problem I faced here. 


I think that the Perspective API model might be biased against or have difficulty understanding nuances of language or text that needs context to be fully understood. For example, I think it might have trouble picking up on sarcasm as well as jokes that might contain toxic words but with context the text would actually be considered non-toxic by most people. The model might also face difficulty grasping cultural differences and what would be considered toxic and non-toxic in other cultures. 
 
