---
slug: "projects/1-rfm.md"
nameOfClass: "projects-items dataProjects"
added: "2022-08-07"
title: "RFM"
video: "true"
listName: "📊 /RFM기반_고객_클러스터링"
popupImageSrc: "country-quiz.webp"
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

    - STP 프레임워크 수립을 위해 고객 세분화 진행
    - 고객과 매출 데이터를a 기반으로 고객 별 RFM 측정 
    - 고객 세분화에 사용할 K-MEANS 군집분석을 위해 사전에 Min-Max scaler 수행 
——
    - RFM을 기반으로 K-MEANS 군집분석 진행 
    - 최적의 군집개수를 선정하기 위해 각 군집 별 실루엣 계수 비교 
    - 실루엣 계수가 비교적 1에 가까우면서 seg별 고객이 고루 분포된 5를 최적의 K로 선정   
——    - 총 구매액합계가 높은 seg1과 구매자별 평균 구매액이 높은 seg2를 타깃으로 설정
    - seg1의 경우 소량이라도 브랜드가 좋은 술을 추천
    - seg5의 경우 명절 전 선물에 대한 수요를 반영하여 선물박스 대량으로 구매에 대한 프로모션 진행