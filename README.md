# sentiment-analysis

## __앞으로 할거__

### ▶ 감성분석 데이터셋

- 감성 대화 말뭉치 (tutorial)  
https://aihub.or.kr/unitysearch/list.do?kwd=%EA%B0%90%EC%84%B1

- 한국어 감정 정보가 포함된 단발성 대화 데이터셋  
- 한국어 감정 정보가 포함된 연속적 대화 데이터셋
- 감정 분류용 데이터셋  
https://aihub.or.kr/unitysearch/list.do?kwd=%EA%B0%90%EC%A0%95  

전처리 방법  
사람 대화, 시스템 응답, 부감정 까자 써보고 정확도 비교

데이터셋 별로 정확도 구해보고, 데이터 병합하는 방법도 생각


### ▶ 텍스트 처리  
텍스트 마이닝이 꼭 필요?

(감성 대화 말뭉치는) 데이터셋이 validation set을 포함하여 다 대화문으로 구성되있는데 평문에 대한 감성분류가 제대로 될 수 있는지  
이게 어려울 경우 평문이랑 대화문을 분리해서 처리 하기 등


### ▶ 언어 모델 공부

- NLP
토큰화 ,Vocab  
데이터셋이 문장 단위로 라벨링 되있는데 토큰화 단위로 뭐가 적합한지  

KoBERT  
토크나이징 함수, 사용되는 파라미터들을 설정, optimizer loss 함수, 스케쥴러  
-특히  learning rate, epochs

- 모델 선정
KoBERT외에 KcBERT, RNN계열..
위에서 말한 평문/대화문에

+코랩에서 학습 시키면 모델 하나 훈련하는데 40분 넘게 걸리고(에포크5), 사용량 제한 걸림
gpu사다 쓰면 더 낫나

### ▶ ML
-성능향상 기법

오버피팅 안되는 선에서 에포크 값조절 
앙상블, 하이퍼파라미터 튜닝 등..

### ▶ 모델의 성능평가
일단 한 문장에 대해서만  validation set  
책이랑 음악을 매칭해줬다고 평가할 수 있는 방법?  

### ▶ 음악 매칭  
라벨로 쓰이는 감정이 거의 부정적인데 음악이랑 적절히 매칭될 수 있는지  
책 장르 까지 추가로 활용하는 방안  

(2학기)
다른 매칭방법? 
검색, 음원 스팩트럼 분석, 코사인 유사도 구하기..  
유튜브 플레이리스트, 멜론 태그별 수록곡
