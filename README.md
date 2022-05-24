# DACON_Korea_Sentence_relation
![20220524_104944](https://user-images.githubusercontent.com/84311270/169932385-ed6622cb-c4a3-4ba9-8409-baed70da6217.png)  


한국어 문장 관계 분류 경진대회에 참여하여 한 쌍의 문장은 Natural Language Inference Dataset을 활용한 Premise와 Hypothesis로 구성되어 있는 데이터를 분석하였습니다. premise 문장을 참고해 hypothesis 문장이 참인지(Entailment), 거짓인지(Contradiction), 혹은 참/거짓 여부를 알 수 없는 문장인지(Neutral)를 판별하는 것이 목적이였습니다.

## Dataset
1. train_data.csv  
├ Index : train data index  
├ Premise : 실제 Text  
├ Hypothesis : 가설 Text  
└ Label : 참(Entailment) 또는 거짓(Contradiction) 또는 중립(Neutral)  

2. test_data.csv  
├ Index : test data index  
├ Premise : 실제 Text  
├Hypothesis : 가설 Text  
└Label : 추론해야 하는 Label 값  

3. sample_submission.csv  
├ Index : test data index  
└Label : 추론해야 하는 Label 값  

## Model
klue/roberta-large 모델을 사용하였으며 StratifiedKFold를 사용하여 모델을 검증하였습니다.


## Results 
Public Score : 0.88, Private Score : 0.87635로 최종 42등으로 상위 10% 안에 들며 대회를 마무리하였습니다.   

![20220524_105148](https://user-images.githubusercontent.com/84311270/169932529-de69fc52-fb53-4be9-a2f4-cab4d1bef095.png)
