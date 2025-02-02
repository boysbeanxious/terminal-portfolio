---
slug: "experience/sysproof.md"
added: "2017-01-09"
video: "true"
nameOfClass: "projects-items"
title: "시스템 검증"
listName: "👩‍💻 /시스템 검증"
techIcons: [
        "java",
        "spring",
        "oracle",
        "linux"
      ]
---

매일 아침, 출근과 함께 나의 하루를 시작한 업무가 바로 시스템 검증이다.   
개발도 무척이나 중요하지만, 시스템이 안정적으로 운영되지 않는다면 개발은 무의미하다.    
무게를 지탱하는 블럭이 흐트러지면 새로 쌓은 블럭으로 인해 전체가 와르르 무너지는 젠가게임처럼,  
불안정안 시스템에 신규 개발 건을 반영하면 장애를 맞이할 수 있기 때문에 시스템이 잘 운영되고 있는지 검증 과정을 거치게된다.   
아래 세개의 업무가 가장 중요하게 검증했던 요소이다.    
시스템의 근간을 이루는 서버부터 데이터, 그리고 배포 시스템까지 확인하면 그때부터 본격적인 업무를 시작할 수 있다.    
   
   
#### [서버 가용성 관리]()  
    ✔︎ WAS서버 가용성 관리를 위하여 일주일이 지난 로그의 경우 삭제하는 배치 프로그램 작성 및 모니터링    
    ✔︎ DB서버 가용성관리를 요일별 파티션을 생성하고 과거 파티션을 삭제하는 배치 프로그램 작성 및 모니터링    
        
#### [데이터 품질 관리]()  
    ✔︎ 일 검증 배치 프로그램 작성하여 담당업무 테이블의 데이터 품질 관리  
    ✔︎ 수수료 지급금액에 대한 이상치 감지하여 특이사항 발생 시 모니터링 기능 강화        
     
#### [배포 안정성 관리]()  
    ✔︎ 통합 테스트 환경의 소스코드를 매일 롤백하여 운영환경과 동일한 상태로 테스트 가능하도록 구성  
    ✔︎ 배포 시 위험한 프로그램을 배포하는 경우 담당자에게 push 알림 전송 모니터링  
