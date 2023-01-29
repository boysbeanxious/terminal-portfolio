어릴적, 누구나 한번쯤 접해본 오락실 게임.
모든 게임의 시작을 지키고 있었던 문구는 단 하나다. 

_INSERT COIN_

어느날 문득 100원 짜리 동전 하나로 시작해서 몇천원과 행복을 맞바꾸는것이 오락실 게임과 투자가 닮아있다는 생각이 들었다.  돈을 넣어야 시작할 수 있는것 부터 시작하면 끝내기 힘들다는 점까지 닮은 점이 한둘이 아니었다. 

그래서 프로젝트 INSERT COIN을 시작하게 되었고, 현재 Trilogy까지 완성한 상황이다.  
Trilogy에서 멈추지 않고 자연어처리를 기반으로 한 주식 종가 예측까지 계속 이어갈 예정이다.

### INSERT COIN I.  
✔︎ 최초 INSERT COIN 프로젝트  
✔︎ 데이콘에서 주최하는 '2021 금융데이터 활용경진대회' 대회에 팀명 INSERT COIN 으로 참여  
✔︎ 코로나 이후는 하락장이라는 가설설정과 AR모형을 통한 오차 최소화  
✔︎ 알고리즘 기반 주식 자동 매매 프로그램을 개발하여 최종 15위 달성  


### INSERT COIN II.  
✔︎ 첫번째 프로젝트에서 부족한 부분을 채우기 위해 대학원에서 '금융 데이터 분석' 수업 수강
✔︎ 환율 이외의 GDP성장률, 유가 증감률과 같은 거시 지표 활용
✔︎ 시계열 데이터로 선형회귀 수행
✔︎ 계량경제학을 통해 가격의 비정상성을 이해하고 증감율 기반으로 예측

### INSERT COIN III
✔︎ 앞서 진행한 프로젝트를 기반으로 KOSPI/S&P500 지수 예측 프로젝트 진행 
✔︎ 차분을 통해 계산된 증감률, 기술지표와 거시지표를 feature로 활용
✔︎ 예측이 아닌 상승과 하락의 분류로 변경하여 진행
✔︎ 높은 정확도를 위한 최적 모델 탐색



### INSERT COIN I

<span style ='color:#2D3748; background-color:#F7DDBE'> ✔︎ INSERT COIN I</span><br>
<div float: left; width: 100%;">
    <img src="https://boysbeanxious22.netlify.app/insert_coin_1.png" style="float: left; width: 100%;">
</div>

<span style ='color:#2D3748; background-color:#F7DDBE'> ✔︎ INSERT COIN II</span><br>
<div float: left; width: 100%;">
    <img src="https://boysbeanxious22.netlify.app/insert_coin_2.png" style="float: left; width: 100%;">
</div>

<span style ='color:#2D3748; background-color:#F7DDBE'> ✔︎ INSERT COIN III</span><br>
<div float: left; width: 100%;">
    <img src="https://boysbeanxious22.netlify.app/insert_coin_3.png" style="float: left; width: 100%;">
</div>


<div style = "padding: 5px 1px 2px 3px;">  
<div style="display:inline-block;vertical-align:top;">
    <img src="https://boysbeanxious22.netlify.app/insert_coin_1_1.png" height="200px" style="vertical-align:middle;">
</div>
<div style="display:inline-block;vertical-align:middle">
    <p>
                <span style ='color:#2D3748; background-color:#F7DDBE'> ✔︎ 예측 대상 일은 하락장일 것이다</span><br>
                . 지수와 환율이 서로 상반된 움직임을 보임<br>
                . 예측하는 2021년 하반기의 경우 환율 상승<br>
                . 예측 대상일을 하락장으로 가정하여 큰 폭의 하락을 보인 2019년 12월부터의 데이터 활용<br>
    </p>
</div>
<div style="display:inline-block;vertical-align:top;">
    <img src="https://boysbeanxious22.netlify.app/insert_coin_1_3.png" height="200px" style="vertical-align:middle;">
</div>
<div style="display:inline-block;vertical-align:middle">
    <p>
		. 종가자체로 예측하기 위해 자기회귀모형 사용<br>
		. 최적의 파라미터 확인을 위해 grid search 진행<br>
		. RMSE기준으로 잔차가 가장 적은 파라미터 선택<br>
		. 최적의 모델 기준으로 종가 예측<br>
    </p>
</div>
<br>
<div style="display:inline-block;vertical-align:top;">
    <img src="https://boysbeanxious22.netlify.app/insert_coin_1_2.png" height="200px" style="vertical-align:middle;">
</div>
<div style="display:inline-block;vertical-align:middle">
    <p>
                . 일자별로 주식 종가와의 상관 계수 확인<br>
                . D-1, D-2, ---, D-n 일자의 종가가 D-Day의 종가와 가장 높은 상관관계를 보임 <br>
                . 크롤링한 데이터 대신 종가기준으로 예측 진행 <br>
    </p>
</div>
<br>
</div>



 
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
