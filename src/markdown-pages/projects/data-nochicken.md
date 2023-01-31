---
slug: "projects/4-nochicken.md"
nameOfClass: "projects-items dataProjects"
added: "2021-12-11"
title: "치킨집은 정답이 아니다"
video: "false"
listName: "📊 /치킨집은_정답이_아니다"
popupImageSrc: "chicken.png"
popupImageAlt: "Country Quiz screenshot"
techIcons: [
        "react",
        "html5",
        "css3",
        "tailwindcss",
      ]
---

이 프로젝트를 진행하게 된 것은 취업 준비 생 시절 나를 웃게 한 사진 덕분이다.

<div style="display:inline-block;vertical-align:top;">
    <img src="https://boysbeanxious22.netlify.app/jinro.jpg" height="300px" style="vertical-align:middle;">
</div>
  
어떤 선택을 하든 결국 치킨 집으로 귀결된다는 것이 안정감을 주면서도 궁금증을 자아낼 수 밖에 없었다.  
물론 그 당시 지금보다도 치킨에 대한 인기가 컸지만 도대체 치킨집이 무엇이길래 다른 음식점도 아닌 치킨인지 알수 없었다. 
  
그래서 한번 가정해보았다. 
  
_내가 만약에 카이스트 홍릉 주변에서 요식업을 하게 된다면, 어떤 요식업을 해야하는걸까?_  
  
서울시에서 제공하는 데모그래픽 정보와 상권 데이터를 기반으로 카이스트 홍릉 주변 요식업의 매출을 예측해 보았다. 
  
### [외식업 창업자를 위한 상권분석 및 업종추천](https://drive.google.com/file/d/1JO6mgll54LVWG7mRILmkn4WtV7QBoex8/view)  
__step1.업종별 매출에 영향을 미치는 요인 탐색__  
✔︎ 외식 업종 별 매출액에 영향을 미치는 요인이 서로 상이하다고 가정  
✔︎ 업종별 매출을 y로 설정하고 각 변수 X와 y의 OLS 수행하여 R2값 확인   
✔︎ 업종별 유의미한 상관관계를 보인 변수 추출  
  
__step2.카이스트 주변과 유사한 상권 군집화__  
✔︎ 앞서 확인한 업종별 유의미한 변수 전체 기준 군집분석 진행   
✔︎ 카이스트 주변 상권이 속한 클러스터 특성 확인  
✔︎ 다른 상권에 비해 생활인구가 적지만 필수소비재 (병원, 식료품)에 대한 지출이 높은 군집  
  
__step3.카이스트 주변 외식업 예상 매출 TOP4__
✔︎ 업종별 유의미한 변수 기반으로 회귀분석 진행  
✔︎ 최적의 결과 도출을 위해 업종별로 가장 낮은 RMSE 점수를 보이는 모델 선택  
✔︎ 홍릉 카이스트 주변 상권 기준으로 점포별 예상매출이 가장 높은 업종은 한식음식점   

