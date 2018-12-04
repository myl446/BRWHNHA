1. DDS is the diseases semantic similarity matrix, MMS is the miRNAs similarity functional matrix, M is the known miRNA-disease associations.
2. Similarity is used to calculated the Gaussian interaction profile kernel similarity, and integrate the Gaussian interaction profile kernel similarity into DDS and MMS。
3. reSimilarity is used to recalculate the similarity of miRNAs.
4. normFun1 is used to normalize DDS and MMs.
5. BiRWHMDA is the code of unbalance bi-random walk on heterogeneous network. The associations probability matrix will be obtained by inputting the diseases similarity, the miRNAs similarity and the known miRNA-disease associations.
6. main_HeatS_ProbS and HeatS_ProbS_recommendations are the code of hybrid recommendation algorithm. The miRNA-disease transition probability matrix is obtained by inputting the known miRNA-disease associations. 
7. FivefoldcrossValidation is the code of five-fold cross-validation. For a given, the known miRNA-disease association is divided into five equal subset by inputting the number of i from 1 to 22.
8. Roc _curve is used to calculate the AUC value.
9. repition is used to repeat five-fold cross-validation 100 times, and finally get the average AUC of 100 five-fold cross-validation.

Running the main function of repition will directly obtain the AUC of 22 disease that associated with at least 60 miRNAs.
