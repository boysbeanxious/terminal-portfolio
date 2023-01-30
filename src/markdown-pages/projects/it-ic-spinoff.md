---
slug: "projects/2-ic-spinoff"
added: "2021-08-02"
nameOfClass: "projects-items itProjects"
title: "insert coin : spin off"
listName: "📱 /insert_coin_spinoff"
video: "false"
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
데이터 분석을 아장아장 배우던 때 발생한 코시국. 사람마다 다르겠지만 코시국하면 가장 많이 들어본 단어는 떡상 혹은 떡락 아닐까? 주식과 코인으로 동학개미들의 막대한 자본이 들어가면서 근 2년간 불시장을 형성했다. 나 포함 내 주변에서 주식의 '주' 자도 꺼내지 않던 친구들이 만나면 종목추천과 MTS를 열어보기 바빴다. 이러던 도중 몇가지 의문이 생겼다.

✔️ 다들 어디서 정보를 얻어서 주식이 오를거라고 판단하는걸까?  
✔️ 카더라가 주식을 움직이는걸까?  
✔️ 모든 정보가 사실과 다를수 있는데 정확하다는 판단은 어떻게 하는걸까?  
✔️ 주식을 움직이는 힘은 무엇일까?  
  
이 모든 의문을 해결할 수 있는 방법은 단 한가지였다!  
  
_수많은 데이터 중 어떤 정보가 주식에 가장 큰 영향을 주는지 분석해보자_  

### [spin off : 감정분석을 통한 주가 예측](https://github.com/boysbeanxious/insertcoin)
✔️ client side 없이 Server 기준으로 설계  
✔️ Python으로 개발한 Crawling프로그램으로 수집   
✔️ 텍스트 데이터 기반으로 자연어 분석 처리  
✔️ 감정분석으로 주가 예측이 최종목표  
✔️ 주가에 영향을 줄 것이라고 예상 되는 매체 기준 데이터 수집(뉴스, 종목토론방)  
✔️ 수집한 데이터는 DB에 저장(Elastic Search) 후 자연어 분석 시 사용  
✔️ AWS Pipeline을 사용해 CI/CD 구축   
✔️ 서로 독립적으로 구동되는 MSA서비스를 위해 AWS ESC사용   
✔️ 병렬 프로그래밍이 가능하도록 AWS SQS 적용   
    
