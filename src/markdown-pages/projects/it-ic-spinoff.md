---
slug: "projects/2-ic-spinoff"
added: "2021-08-02"
nameOfClass: "projects-items itProjects"
title: "insert coin : spin off"
listName: "📱 /insert_coin_spinoff"
video: "true"
popupImageSrc: "SunnysideSS.png"
popupImageAlt: "Sunnyside agency screenshot"
popupLiveLink: "https://sunnyside.pantak.net/"
popupGithubLink: "https://github.com/Kielx/Sunnyside"
techIcons: [
        "html5",
        "css3",
        "javascript",
        "react",
        "tailwindcss",
      ]
---

    - client side 없이 Server 기준으로 설계
    - Python으로 개발한 Crawling프로그램으로 수집 
    - 텍스트 데이터 기반으로 자연어 분석 처리
    - 감정분석으로 주가 예측이 최종목표
——
 

    - 주가에 영향을 줄 것이라고 예상 되는 매체 기준 데이터 수집(뉴스, 종목토론방)
    - 수집한 데이터는 DB에 저장(Elastic Search) 후 자연어 분석 시 사용
—-

    - AWS Pipeline을 사용해 CI/CD 구축 
    - 서로 독립적으로 구동되는 MSA서비스를 위해 AWS ESC사용 
    - 병렬 프로그래밍이 가능하도록 AWS SQS 적용 
    
