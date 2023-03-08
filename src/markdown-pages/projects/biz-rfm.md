---
slug: "biz-project/rfm.md"
nameOfClass: "projects-items bizProjects"
added: "2022-08-07"
title: "RFM기반_마케팅_전략_수립"
video: "false"
listName: "📋 /RFM 기반 마케팅 전략 수립"
popupImageSrc: "rfm.png"
popupImageAlt: "Country Quiz screenshot"
techIcons: [
        "python",
        "jupyter",
        "postgresql"
      ]
---

이론으로 배운 모델링을 실제 데이터에 접목하여 비즈니스 관점에서 해석한 첫번째 프로젝트이다.   
전통주를 판매하는 온라인 플랫폼 '술담화'와 함께 한 프로젝트로 그들의 니즈는 명확했다.    
  
_"매출을 올리고 싶습니다"_  

회사의 매출 데이터가 대외비였던 만큼, 모델링에서 그치치 않고 바로 적용 가능한 자문을 하기 위해 노력했다.  
그 중에서도 마케팅 관점에서 고객 분석을 위해 매출 데이터 기반으로 RFM을 산정하여 고객 클러스터링을 진행하였고  
데모그래픽 기반으로 클러스터의 특성을 파악하여 전략을 세웠다.  

### [담화마켓 성장을 위한 데이터 분석 프로젝트](https://drive.google.com/file/d/17S0AACogD0NuWdkyENVeCxI7nFIRf5hF/view?usp=sharing  "클릭하여 상세 문서를 다운받을 수 있습니다.")  
__step1.매출 기반 RFM 산정__  
✔︎ STP 프레임워크 수립을 위해 고객 세분화 진행  
✔︎ 고객과 매출 데이터를 기반으로 고객 별 RFM 측정   
✔︎ 고객 세분화에 사용할 K-MEANS 군집분석을 위해 사전에 Min-Max scaler 수행  
  
  
__step2.최적의 군집 개수 탐색__  
✔︎ RFM을 기반으로 K-MEANS 군집분석 진행  
✔︎ 최적의 군집개수를 선정하기 위해 각 군집 별 실루엣 계수 비교  
✔︎ 실루엣 계수가 비교적 1에 가까우면서 seg별 고객이 고루 분포된 5를 최적의 K로 선정  
  
  
__step3.고객 seg별 전략 수립__  
✔︎ 총 구매액합계가 높은 seg1과 구매자별 평균 구매액이 높은 seg2를 타깃으로 설정  
✔︎ seg1의 경우 소량이라도 브랜드가 좋은 술을 추천  
✔︎ seg5의 경우 명절 전 선물에 대한 수요를 반영하여 선물박스 대량으로 구매에 대한 프로모션 진행  
