# CA04
Ensemble Methods applied to Census Data. Continuation of work done in CA03. I have not included the rest of the details for this Readme, so as to focus attention on the conclusion from my findings on assessing the ensemble methods. If you need to refer to sections before the ensemble method, kindly refer to CA03 repository. 

## Compare Performance

For the disucssion to follow, please refer to the table ensemble_scores that can be found below. I took the list of results from all four models and used the MAX function to extract the most accurate result for accuracy and AUC for each model. Next, I created a dictionary called "__best_scores__" and a row index with the labels for the performance measures _Accuracy_ and _AUC_. Finally, I created a Data Frame called __ensemble_scores_df__, which lists the best performance measures.

In summary, XGB Boost has the most balanced score out of all the ensemble methods. It is a close second in accuracy at 84.36% and in pole position in AUC with a score of 89.21%. This performance demonstrates why XGB is widely adopted in industry. In contrast, AdaBoost unsurprisingly performed the worst with an accuracy of 83.86% and an AUC of 74.58%. It is often criticised for generalizing, which makes it susceptible to errors when the data has noise or outliers. Based on these results, XGB Boost is the preferred ensemble method going forward.
