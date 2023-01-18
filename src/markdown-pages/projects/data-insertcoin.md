---
slug: "projects/2-insert-coin.md"
nameOfClass: "projects-items dataProjects"
added: "2021-12-11"
title: "Insert Coin"
video: "true"
listName: "📊 /insert_coin"
popupImageSrc: "photo.jpeg"
popupImageAlt: "Country Quiz screenshot"
popupLiveLink: "https://country-quiz.pantak.net/"
popupGithubLink: "https://github.com/Kielx/country-quiz"
techIcons: [
        "react",
        "html5",
        "css3",
        "tailwindcss",
      ]
---

### INSERT COIN I

<div style="display:inline-block;vertical-align:middle;">
    <img src="https://boysbeanxious22.netlify.app/insert_coin_1_1.png" height="200px" style="vertical-align:middle;">
</div>
<div style="display:inline-block;">
    <p>
                <span style ='background-color:#F7DDBE'> ✔︎ 예측 대상 일은 하락장일 것이다</span><br>
                . 지수와 환율이 서로 상반된 움직임을 보임<br>
                . 예측하는 2021년 하반기의 경우 환율 상승<br>
                . 예측 대상일을 하락장으로 가정하여 큰 폭의 하락을 보인 2019년 12월부터의 데이터 활용<br>
    </p>
</div>
<br>
<div style="display:inline-block;vertical-align:middle;">
    <img src="https://boysbeanxious22.netlify.app/insert_coin_1_3.png" height="200px" style="vertical-align:middle;">
</div>
<div style="display:inline-block;">
    <p>
		. 종가자체로 예측하기 위해 자기회귀모형 사용<br>
		. 최적의 파라미터 확인을 위해 grid search 진행<br>
		. RMSE기준으로 잔차가 가장 적은 파라미터 선택<br>
		. 최적의 모델 기준으로 종가 예측<br>
    </p>
</div>
<br>

<div style="display:inline-block;vertical-align:middle;">
    <img src="https://boysbeanxious22.netlify.app/insert_coin_1_2.png" height="200px" style="vertical-align:middle;">
</div>
<div style="display:inline-block;">
    <p>
                . 일자별로 주식 종가와의 상관 계수 확인<br>
                . D-1, D-2, ---, D-n 일자의 종가가 D-Day의 종가와 가장 높은 상관관계를 보임 <br>
                . 크롤링한 데이터 대신 종가기준으로 예측 진행 <br>
    </p>
</div>
<br>




 
#### INSERT COIN II
    - 거시 지표 기반의 환율 예측 진행
    - 계량경제학을 통해 가격의 비정상성을 이해하고 증감율 기반으로 예측
    - 환율 이외의 GDP성장률, 유가 증감률과 같은 거시 지표 활용
    - 시계열 데이터로 선형회귀 수행
    
#### INSERT COIN III
    - 앞서 배운 내용을 기반으로 KOSPI/S&P500지수 예측 
    - 차분을 통해 계산된 증감률 기술지표와 거시지표를 feature로 활용
    - 예측이 아닌 상승과 하락의 분류로 변경하여 진행
    - 높은 정확도를 위한 최적 모델 탐색
