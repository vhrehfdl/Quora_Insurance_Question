# Purpose
Quora 질문이 부적절한 질문인지 binary classification.

여기서 부적절한 질문은 성적인 질문, 인종차별적 질문, 정치적인 질문 등을 의미한다.



# Data
## Data example
text | label
|:--------|:--------:|
What type of wildlife can be found in the Brazilian Pantanal?|0
Is the US Federal Reserve a private enterprise?|0
"I celebrated Trump's victory anniversary by hunting 7 deers for food, what do liberals think about it?"|1
Why did Japan want to kill Jewish?|1
What are the types of rattlesnakes in Texas?|0



# Model 
1. BI_LSTM 
  * CuDNN 사용한 Bi LSTM 레이어 2개 쌓았다.
2. TextCNN 
  * filter_size : 3, 4, 5
  * filter_num : 128