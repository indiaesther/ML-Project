# ML-Project
비정형 데이터를 활용한 인공지능 자연어 전처리과정 201127-210226

기업 데이터 및 기업이 개발하고자 하는 R&D 목표 데이터는 비정형이다. 
기업은 적합한 지원사업을 찾는데 어려움을 겪거나, 적합하다 생각했는데 요건이 충족하지 않는 것을 확인하고 중단되는 경우가 비일비재하다. 
이러한 어려움을 해결하기 위해 사전에 기업에게 적합한 사업을 추전해줄 수 있는 알고리즘을 개발하게 되었다. 기 선정된 기업과 유사한 요건의 기업이 다음 지원사업에서 역시 선정될 가능성이 높다는
가정을 세웠다.


## 추천 시스템 구조
![RD01](https://user-images.githubusercontent.com/68997381/120438370-40997980-c3bc-11eb-9913-2a08bd27a8cc.PNG)


## 데이터 수집
![RD02](https://user-images.githubusercontent.com/68997381/120438581-85251500-c3bc-11eb-842c-d09d7e516bbb.PNG)


## 팀원

신성은, 이정우, 강시내

## 개발기간 

- 기간: 2021.01.28 - 2021.02.26

## 적용기술

**Programming Language**
- Python

**Library**
- SKlearn
- Pandas
- numpy
- matplotlib
- seaborn
- Selenium
- konlpy
- nltk
- krwordrank
- WordCloud
- gensim


## 구현 기능 및 개인 역할

**신성은**

- NTIS 기 선정된 연구과제 크롤링
- 데이터 전처리
- Okt, Hannanum, Kkma, Kr-WordRank 토큰화 및 키워드 추출
- WordCloud를 이용한 불용어 사전 구축
- 키워드를 이용한 연구과제 소관부처 분류 모델
- 분류 모델 성능 개선


## 나의 결과물: 매출현황 페이지 구현

### 1. NLTK 패키지를 이용한 키워드 WordCloud 시각화
![RD03](https://user-images.githubusercontent.com/68997381/120440059-2b254f00-c3be-11eb-9a36-eebdb34bcc2b.PNG)
![RD04](https://user-images.githubusercontent.com/68997381/120440066-2d87a900-c3be-11eb-8da1-66b84f0c1750.PNG)


### 2. Pipeline 생성
![RD05](https://user-images.githubusercontent.com/68997381/120440125-3c6e5b80-c3be-11eb-8323-637b6268d0ee.PNG)


### 3. 하이퍼파라미터 튜닝
![RD07](https://user-images.githubusercontent.com/68997381/120440232-4f812b80-c3be-11eb-9f77-41cec8a53209.PNG)

<성능측정 결과>
![RD06](https://user-images.githubusercontent.com/68997381/120440413-7b041600-c3be-11eb-9f27-d50d476974b8.PNG)


### 4. 성능이 높은 알고리즘을 이용해 토큰화 조합 찾기
<성능측정 결과>
![RD08](https://user-images.githubusercontent.com/68997381/120440479-8fe0a980-c3be-11eb-96cd-9798ff8f6cac.PNG)


<ROC Curve>
![RD10](https://user-images.githubusercontent.com/68997381/120441011-1ac1a400-c3bf-11eb-94a6-3fe4e54bbba8.PNG)
  
### 5. 성능 높은 알고리즘과 토큰화 조합으로 성능 재측정
<성능측정 결과>
![RD09](https://user-images.githubusercontent.com/68997381/120440610-b1419580-c3be-11eb-8a0e-328718611b4e.PNG)

<ROC Curve & Confusion Matrix>
  - SVC VS. Linear SVC -
  ![RD11](https://user-images.githubusercontent.com/68997381/120440829-e948d880-c3be-11eb-8401-280a279ce8f2.PNG)






