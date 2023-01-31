---
slug: "projects/2-insert-coin.md"
nameOfClass: "projects-items dataProjects"
added: "2021-12-11"
title: "Insert Coin Trilogy"
video: "false"
listName: "📊 /insert_coin"
popupImageSrc: "inert_coin.png"
popupImageAlt: "Country Quiz screenshot"
techIcons: [
        "python",
        "jupyter"
      ]
---


누구나 한번쯤 접해본 오락실 게임.  
모든 게임의 시작을 지키고 있었던 문구는 단 하나다. 

_INSERT COIN_

어느날 문득, 100원 짜리 동전 하나로 시작해서 몇천원과 행복을 맞바꾸는 오락실 게임과 투자가 닮아있다는 생각이 들었다. 돈을 넣어야 시작할 수 있는것 부터 시작하면 끝내기 힘들다는 점까지 비슷한 점이 한둘이 아니었다. 

그래서 프로젝트 명 INSERT COIN을 시작하게 되었고, 현재 3편까지 완성한 상황이다.  
Trilogy에서 멈추지 않고 자연어처리를 기반으로 한 주식 종가 예측까지 계속 이어갈 예정이다.

  
### [INSERT COIN I : 주식 종료가격 예측](https://drive.google.com/file/d/1K7sl6rLGxETRN9r5hpAT_8jORxX2DR-H/view)    
__step1.예측 대상 일은 하락장일것이다__    
✔︎ 지수와 환율이 서로 상반된 움직임을 보임    
✔︎ 예측하는 2021년 하반기의 경우 환율 상승    
✔︎ 예측 대상일을 하락장으로 가정하여 큰 폭의 하락장을 보인 2019년 12월부터의 데이터 활용    
  
  
__step2.종가는 종가다__  
✔︎ 일자별로 주식 종가와의 상관 계수 확인  
✔︎ D-1, D-2, ---, D-n 일자의 종가가 D-Day의 종가와 가장 높은 상관관계를 보임    
✔︎ 크롤링한 데이터 대신 종가기준으로 예측 진행    
  
  
__step3.자기회귀(AR)모형__  
✔︎ 종가자체로 예측하기 위해 자기회귀모형 사용  
✔︎ 최적의 파라미터 확인을 위해 grid search 진행      
✔︎ RMSE기준으로 잔차가 가장 적은 파라미터 선택   
  
### [INSERT COIN II : 거시지표 기반의 환율 예측](https://docs.google.com/presentation/d/12MXZBETpu6qNdGp8aQCni2mf_Hp7PZ4T/edit)    
__step1.환율 대신 환율 증감률__  
✔︎ 환율데이터 예측 프로젝트 진행
✔︎ 환율과 같은 가격 데이터는 비정상성을 가져 예측하기 어렵기 때문에 정상성 확보를 위해 차분 진행 
✔︎ 환율 증감률을 사용하여 정상성 확보  
  
__step2.거시지표 활용__  
✔︎ 명목환율을 예측하는데 실질 환율 활용  
✔︎ 이외 국가별 거시 지표를 표현하는 데이터 수집  
✔︎ 안전자산으로 분류되는 금과 유가도 환율 예측 지표에 추가   
  
__step3.시계열 데이터로 선형회귀__  
✔︎ 날짜를 인덱스로 가지는 데이터셋 생성  
✔︎ 계절성을 감안하여 1년 후 명목환율 증감률을 종속변수로 지정    
✔︎ OLS 선형회귀 분석 수행하여 변수 별 영향력 확인  
  
  
### [INSERT COIN III : KOSPI/S&P500 지수 예측](https://drive.google.com/file/d/1G3d_ViNj8xwgdw0F5mDrtZ6lsoOl2ROt/view)   
__step1.기술지표+거시지표 활용__  
✔︎ 종가만을 활용한 INSERT COINⅠ의 경우 비정상성을 띄는 데이터로 주가 분석 진행  
✔︎ 종가 이외의 볼린저밴드, RSI와 같은 기술지표와 소비자 물가지수, 국제유가 증감률과 같은 거시지표 수집  
✔︎ 정상성 확보를 위해 차분 진행  
  
__step2.상승/하락의 분류 문제로__  
✔︎ 수치를 예측한 INSERT COIN Ⅰ, Ⅱ 에서 보았듯 명확한 증감률을 예측하는 데 한계가 존재  
✔︎ 지수의 상승과 하락으로 문제를 달리 정의 했을 때, 0/1의 분류문제로 변환 가능        
  
__step3.높은 정확도를 위한 최적모델 탐색__  
✔︎ 데이터를 분류하는 데 다양한 모델 존재  
✔︎ 서로 다른 방식으로 분류하는 모델을 선정하여 데이터 학습 진행        
✔︎ 집단지성을 활용하는 Random Forest에서 가장 좋은 점수 도출  

