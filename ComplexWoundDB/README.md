<div align="center">
<p>
   <a align="left" href="recogna.tech" target="_blank">
   <img width="850" src="https://i1.rgstatic.net/ii/lab.file/AS%3A610997660299264%401522684602522_xl"></a>
</p>
</div>

# ComplexWoundDB 
A Database for Automatic Complex Wound Tissue Categorization 

Dataset from "Talita A. Pereira, Regina C. Popim, Leandro A. Passos, Danillo R. Pereira, Clayton R. Pereira, and João P. Papa (2022). ComplexWoundDB: A Database for Automatic Complex Wound Tissue Categorization. The 29th International Conference on Systems, Signals and Image Processing, IWSSIP 2022".

## Classification Results

The following table presents the F1 and Accuracy (Acc) results considering the task of pixel classification three well-known supervised classifiers, i.e., Naive Bayes, Logistic Regression, and Random Forest, over the masks provided by expert #4. Values in bold stand for the best results (similar to the one with the highest average F1 score) according to the Wilcoxon signed-rank test with 5% of significance.

|% Train |Metric |Naive Bayes|Logistic Regression|Random Forest
|---                    |---  |---    |---    |---    
|90%      |F1<br>Acc   |0.8889 (0.1088) <br> 0.8888 (0.1087) |0.9652 (0.0315)<br> 0.9526 (0.0431)    |**0.9718 (0.0252)** <br> 0.9698 (0.0269)
|80%      |F1<br>Acc   |0.8888 (0.1087) <br>  0.8941 (0.0959) | 0.9653 (0.0312) <br> 0.9529 (0.0425) | **0.9718 (0.0251)** <br> 0.9698 (0.0268)
|70%      |F1<br>Acc   |0.8885 (0.1087)  <br> 0.8940 (0.0958)| $0.9654 (0.0312)  <br> 0.9530 (0.0424)| **0.9717 (0.0252)**  <br>0.9697 (0.0267)
|60%      |F1<br>Acc   |0.8883 (0.1088)  <br> 0.8939 (0.0958)| 0.9654 (0.0312)  <br> 0.9530 (0.0424)| **0.9716 (0.0252)**   <br> 0.9695 (0.0269)   
|50%      |F1<br>Acc   |0.8880 (0.1091) <br> 0.8938 (0.0960)| 0.9654 (0.0312) <br> 0.9531 (0.0424) | **0.9714 (0.0256)** <br>0.9692 (0.0273)
|40%     |F1<br>Acc  |0.8883 (0.1090) <br> 0.8940 (0.0959)| 0.9654 (0.0312) <br>0.9531 (0.0424) | 0.9712 (0.0258)  <br>  0.9689 (0.0276)
|30%     |F1<br>Acc  |0.8878 (0.1096) <br> 0.8937 (0.0963) | 0.9655 (0.0312) <br> 0.9531 (0.0423) | 0.9710 (0.0259) <br>   0.9685 (0.0278) 
|20%     |F1<br>Acc  |0.8880 (0.1092) <br> 0.8939 (0.0961) | 0.9655 (0.0311) <br> 0.9531 (0.0424) | 0.9705 (0.0262) <br>  0.9678 (0.0284)  
|10%     |F1<br>Acc  |0.8883 (0.1089) <br> 0.8940 (0.0963 | 0.9654 (0.0313) <br> 0.9531 (0.0424  | 0.9694 (0.0272) <br>   0.9664 (0.0295

## Classified Images

Some dataset samples: the first column figures the original image, annotation by expert #4 in the middle, and tissue classification by Random Forest on the righter column. The first row depicts dataset image #8, followed by dataset images #15, and #19.
<div align="center">
<p>
   <img width="850" src="https://drive.google.com/uc?export=view&id=1SwPYsVQX6RtQhrB805AZ877QTXebry_k"></a>
</p>
</div>
