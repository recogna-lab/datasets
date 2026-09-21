<div align="center">
<p>
   <a align="left" href="recogna.tech" target="_blank">
   <img width="570" src="https://i1.rgstatic.net/ii/lab.file/AS%3A610997660299264%401522684602522_xl"></a>
</p>
</div>

# ComplexWoundDB 

ComplexWoundDB is a database for automatic complex wound tissue categorization. If you use it, please cite our paper below: 

"Talita A. Pereira, Regina C. Popim, Leandro A. Passos, Danillo R. Pereira, Clayton R. Pereira, and João P. Papa. *ComplexWoundDB: A Database for Automatic Complex Wound Tissue Categorization.* In Proceedings of the 29th International Conference on Systems, Signals and Image Processing, pp. 1-4, 2022".

## Repository structure

| Directory | Description |
|-----------|-------------|
| [`diabetic-foot/`](diabetic-foot/) | Contains images related to diabetic foot ulcers. |
| [`pressure-ulcers/`](pressure-ulcers/) | Contains pressure ulcer images and corresponding annotations. |
| [`skin-lesions/`](skin-lesions/) | Contains images of different types of skin lesions. |


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


## Patient-Image Information

The table below displays some information from each patient and its corresponding image.

| **Image** | **Patient** | **Time-point<br>(2017)** | **Anatomical location** /<br>**Wound** | **WOUND ID**<br>(patient-location) |
|:-----:|---------|----------------------|--------------------------------|-------------------------------|
| 01 | Patient 01 | 09 September | Right trochanter | 01-RT |
| 02 | Patient 02 | 03 August | Sacral | 02-S |
| 03 | Patient 02 | 03 August | Right trochanter | 02-RT |
| 04 | Patient 02 | 06 June | Sacral | 02-S |
| 05 | Patient 03 | 04 November | Left lateral malleolus | 03-LLM |
| 06 | Patient 03 | 04 November | Right medial malleolus | 03-RMM |
| 07 | Patient 03 | 04 November | Posterior right lower leg | 03-PRLL |
| 08 | Patient 03 | 28 June | Right medial malleolus | 03-RMM |
| 09 | Patient 04 | 12 April | Sacral | 04-S |
| 10 | Patient 04 | 17 August | Right heel | 04-RH |
| 11 | Patient 05 | 31 March | Left lateral malleolus | 05-LLM |
| 12 | Patient 05 | 31 March | Sacral | 05-S |
| 13 | Patient 05 | 31 March | Right trochanter | 05-RT |
| 14 | Patient 05 | 31 March | Left trochanter | 05-LT |
| 15 | Patient 05 | 19 April | Sacral | 05-S |
| 16 | Patient 05 | 19 April | Right trochanter | 05-RT |
| 17 | Patient 05 | 19 April | Left trochanter | 05-LT |
| 18 | Patient 05 | 22 June | Sacral | 05-S |
| 19 | Patient 05 | 22 June | Right trochanter | 05-RT |
| 20 | Patient 06 | 30 January | Left trochanter | 06-LT |
| 21 | Patient 06 | 09 June | Sacral | 06-S |
| 22 | Patient 06 | 09 June | Left trochanter | 06-LT |
| 23 | Patient 07 | 03 August | Right heel | 07-RH |
| 24 | Patient 08 | 07 June | Sacral | 08-S |
| 25 | Patient 09 | 30 May | Sacral | 09-S |
| 26 | Patient 10 | 17 March | Left heel | 10-LH |
| 27 | Patient 10 | 17 March | Right lateral malleolus | 10-RLM |