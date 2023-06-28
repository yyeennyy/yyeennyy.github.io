---
title: 2023년 2월
layout: default
grand_parent: TIL
parent: 23년 상반기
nav_order: 2
---


#### **2월:**
#### **SW아카데미-ing**
#### **졸업프로젝트의 시작**
#### **그리고 첫 클라우드 실습(NCP)**

<br>

{: .new-title }
> 2023.02.01 (수)
> 
> jpa 학습 찔끔


{: .new-title }
> 2023.02.02 (목)
> 1. **졸프** - 교수님과 첫미팅 - [간단 정리](https://splendidlolli.tistory.com/580)
> - 졸프 노션 준비 완료!
> 2. **Spring security 개요**


{: .new-title }
> 2023.02.03 (금)
>1. **팀프로젝트 - marker DTO 수정**
>2. **express.js를 처음 사용해봄..!** (연습용으로 해봄)<br>
>    [**webserver | express.js를 경험해보았다 | 이미지 서버 구축하기**](https://splendidlolli.tistory.com/584)
>
>3. **인텔리제이 재부팅에 대한 인식..** (환경변수 reload 때문)<br>
>[블로그에 정리: Intellij 터미널에서 명령어가 안 먹히는 이유](https://splendidlolli.tistory.com/582)



{: .new-title }
> 2023.02.03 (금)
> 
> 대단한 현진이의 도움을 참 많이 받은 날.. 
> 1. **졸프** 관련 정리 (일정 정리, 기술 고민)<br> 초반 계획에 대해서 친구가 많은 아이디어를 줬다.<br>
> 2. **친구가 https://excalidraw.com/ 추천해줘서 써봤는데..**<br> 너무 좋았다! 갑자기 내 그림 퀄리티 급상승했다. <br> 감사! 그림판 빠이..ㅎㅎ
> 3. 친구가 면접대비 글 정리 같이하자고 제안해주었다.<br> https://github.com/back-to-the-basic/interview<br>
카페에서 방법 안내받았다. 신기했다. 정리 잘 해둬야지!


{: .new-title }
> 2023.02.05 (일)
> 
> **java.util.Properties 클래스**를 인식


{: .new-title }
> 2023.02.06 (월)
>1. **Tiled라는 프로그램**을 알게 되었고, 우리 학교를 픽셀로 찍기 시작<br>(우리 팀 프로젝트에 필요한 배경지도 이미지) 재미있었다.
>2. **네이버 클라우드 특강**<br>
클라우드 산업 현황 인식<br>
네이버 클라우드 플랫폼 구경<br>


{: .new-title }
> 2023.02.07 (화) - 네이버 클라우드 특강
>
>[사용한 상품]<br>
>- Compute 상품군 (서버 생성 실습) → **Server**<br>
>- Networking 상품군 (네트워크 생성 실습) → **VPC**<br>
>
>네이버 클라우드 플랫폼에는 다양한 상품이 있음을 인지했다.
>
>**[실습 순서]**<br>
>VPC 생성, 서브넷생성 → 기본적인 네트워크망 구성<br>
>→ 서버생성 & 접속 → 디스크 증설해보기 → 스냅샷 기능 사용해보기
>
>**[웹콘솔!]**<br>
>https://www.ncloud.com/에서 서브계정으로 로그인하고 웹콘솔에 접속하여 실습을 진행했다.<br>
>서버 운영 방법은 크게 3가지가 있는데, 그중 내가 실습한 웹콘솔로 운영이 가장 권장된다(기능 100% 활용 가능) <br>
>(그밖에 CLI, API를 통해서도 운영 가능)<br>
>
>**[서버 생성+운영 실습]**
>**by 웹콘솔 / ServerImage / 유사서버**<br>
>ㄴ> 세가지 방식의 차이점도 직접 보았다. 
>* 유사서버 : 실제 서버에 있는 데이터를 가져오는 것이 아니라, 서버의 인프라 부분만 복제한다고 생각하기
>* 서버이미지로 생성한 서버 : 위 설명과 반대다! vpc, 서브넷, 서버타입.. 다르게 설정 가능!<br>
>
>**[디스크장착(storage) 실습]**<br>
>- 운영중 서버의 storage(disk)를 확인해보았다. df -h<br>
>- storage 이름 뒤에 1, 2 숫자가 붙은 것은, 파티션이다.<br>
>- **디스크는 /dev/xvda1과 /dev/xvda2가 있었다.**<br>
>
> xvda 디스크의 1번은 boot파티션이었고, 2번은 현재 리눅스의 메인루트볼륨이었다.<br>
>이렇게 서버에 장착된 storage(disk)들의 상태를 보기 위해 fdisk -l 명령을 입력했다. 리스트를 확인했다. storage 추가를 더 한다면 현재 있는 xvda에 이어서, xvdb, xvdc.. 이런 네이밍이 될 거라 하셨다.<br>
>**추가로 storage를 등록했다.** 파티션은 자동으로 등록되어지는 것이 아니라 직접 등록해 주어야 한다. 또한 기본적으로 storage를 사용하려면 파티션을 설정해주어야 한다. **파티션을 추가해보았다. xvdb에 파티션 추가**는 다음 명령 순서대로 가능했다.<br>
>fdisk /dev/xvdb → n → 파티션타입 고르기 → 파티션넘버 고르기 → first sector 설정 → last sector 설정 → 세팅완료! 저장(w)<br>
>그리고 fdisk -l로 확인해보면, 추가된 파티션을 확인 가능하다. 
>**storage를 처음 만들면 포맷을 해야 한다. ext4라는 파일시스템으로 포맷을 진행했다.** mkfs.ext4 /dev/xvdb1 를 통하여 파티션 포맷 완료! 이제 서비스에서 이용이 가능해졌다.<br> 
>**파티션을 실제 폴더로 마운트해보자.** data라는 폴더를 만들었고, 마운트하는 순간, data 폴더는 storage가 된다. data로 우리가 만든 storage를 마운트하는 것이다!<br>
>mount /dev/xvdb1 data<br>
>이렇게 디스크장착 실습 완료!<br>
>
>**[오토스케일링]**<br>
>클라우드의 가장 큰 장점인 유연한 인프라 구축을 가능케 한다는 것을 이해!



{: .new-title }
> 2023.02.08 (수) - 네이버 클라우드 특강
>
>[사용한 상품]<br>
>- Database 상품군 (DB서버 생성 실습) → **Cloud DB for MySQL**<br>
>- AI api 상품군 → **nShortURL**<br>
>- Application Services 상품군 → **Cloud Outbound Mailer**<br>
>
>**[현황]**<br>
>클라우드 DB로 전환되는 시장에 있다!<br>
>하이브리드 클라우드! 별도 보관이 필요한 데이터만 private cloud에 저장, 나머지는 public cloud에 저장.<br>
>대기업은 90%, 중견기업은 76% 이상이 이러한 멀티클라우드 도입을 선호.<br>
>
>**[DB서버 생성과 접속 실습]**<br>
> 1. **생성하기**<br>
>DB 서버 생성을 해봤다.
>생성 과정에서 이 DB에 접근할 수 있는 HOST(ip)도 지정할 수 있다. (모두 다 들어올 수 있게(any) 하고싶으면 %로 지정)
>여기서 %로 하더라도, 추후에 별도로 ACG로 다시 접근을 제한해줄 수 있다.
> 2. **접속하기**<br>
>mysql 서버 생성 완료 후, mysql workbench를 통해 방금 만든 cloud DB에 접속해보았다.<br>
>cloud DB서버에 public 도메인을 신청하면, 외부에서 DB서버로 접근할 수 있다. 외부에서 통신하는 데이터는 네트워크 사용량으로 과금이 된다.
> 3. **ACG**<br>
>DB서버를 만들면 ACG가 자동생성된다. Access Control Group이며, 아래 설정을 하게 된다.
>- Inbound 규칙  : 프로토콜, 접근소스, 허용포트 (서버에 접속 가능할 ip를 지정!)
>- Outbound 규칙 : 프로토콜, 목적지, 허용포트 
>백업/복원 실습, fail-over 테스트도 진행!<br>
>
>*그리고! 새로운 ssh 접속 프로그램을 이용해봄 (MobaXterm)



{: .new-title }
> 2023.02.09 (목) - 네이버 클라우드 특강
>
>[사용한 상품]<br>
>>Management & Govermance
>>- Cloud Insight (Monitoring)
>>- Sub Account
>>- Cloud Log Analytics (CLA)<br>
>>
>>Developer Tools 
>>- Terraform을 이용한 naver cloud infra 구축 실습
>>- terraform VPC 구성 및 리눅스서버 자동생성
>
>**[Cloud Insight (Monitoring) 실습과정]**
>1. 새로운 VPC 생성
>2. 그 Server에다가 상세모니터링, 네트워크 모니터링 신청을 해두면
>3. 해당 VPC에 대한 커스텀 대시보드 만들어서 (Monitoring 상품에서 Dashboard) Widget등록시 데이터 설정 단계에서 Target(감시대상)서버를 해당 서버로 할 수 있다. 그리고 '메트릭'을 SERVER/savg_cpu_used_rto 선택하여 항목추가를 해봤다. 그럼 해당 데이터(그래프)를 확인 가능!
>4. 서버 부하 주고 알림받아보기! Notification Recipient에 통보대상자 김예은씨를 등록
>5. Configuration의 Event Rule에서 감시할 이벤트 룰을 적절히 설정한다. 오늘은 CPU 부하에 대해 Email과 SMS 알림이 오도록 설정해봤다.
>6. CPU 부하 발생시키기 -> 김예은씨에게 알림 간다!!
>* 참고: CPU에 부하 발생시키기 : 해당 서버에 ssh 접속해서 -> EPEL 레포지토리를 설치했다 (yum install epel-release) -> 부하 tool을 설치했다 (yum install stress) -> CPU 부하를 진행 (stress -c 2)
>
>
>**[Sub Account 실습 과정]**<br>
>서브계정 만들고 권한 제한을 줘봤다.<br>
>콘솔 창 접근 제한 등!<br>
>
>**[Cloud Log Analytics(CLA) 실습 과정] (쉽고 간편한 로그조회!)**
>1. CLA -> Subscription에서 CLA 구독 신청!
>2. CLA -> Management에서 해당서버에 로그수집 설정!
>>네이버에서는 다양한 Log Template를 제공한다.<br>
>>실습때는 SYSLOG랑 APACHE Log Template을 추가했다.<br>
>>다음의 로그 경로가 자동 등록되었다.<br>
>>Syslog의 log경로: /var/log/messages<br>
>>Apache의 log경로: /var/log/httpd/error_log<br>
>>                    /var/log/httpd/eccess_log<br>
>>커스텀 로그도 물론 직접 등록 가능!<br>
>3. 해당서버에 Agent 설치하는 방법이 안내된다. (ssh접속 후 명령어를 통해 설치했음)<br>
>* 참고! 해당 서버에서 Apache 로그를 찍어보려는 상황인데 Apache 설치가 안되어있는 상황이라 yum install httpd -y 해주었다.
>4. 해당서버의 공인ip로 웹브라우저로 접속했다. 
>* (잠깐! 먼저 서비스를 start해줘야 함 => systemctl start httpd.service)
>* (그리고 당연히 해당 서버에 ACG의 inbound 설정도 해줘야 함. http는 80포트를 사용하기 때문에, 80포트 inbound 열어줘야 함)
>5. 새로고침 여러번 눌러.... Apache 로그가 찍히도록 했다!
>6. CLA -> Dashboard에 들어가면 로그확인 가능!!!
>* 참고 : 서버에 CLA Agent를 설치한 상황이라면, ssh콘솔통해 서버접속해서 로그를 직접 확인할 수도 있다. <br>
>(웹콘솔로 CLA -> Dashboard 접속할 필요 없이)<br>
>cd /var/log/httpd/ -> cat access_log<br>
>이런 식으로 log 직접 들어가서 확인 가능!<br>
>* CLA -> Search 기능으로 다양하게 로그 검색도 가능<br>
>
> **[Terraform]**<br>
>- Dev Tool로서 제공되는 오픈소스이다.<br>
>- 인프라에 대한 형상관리 툴!<br>
>- 필요성? VPC 생성 등을 클릭으로 하기 귀찮고 오래걸리고 실수가능성도 있는데, 정형화된 코드로 인프라를 쉽게  구성할 수 있다.<br>
>
>**[Terraform VPC 구성 및 Server(Linux) 자동 생성]**<br>
>VPC만들면 Subnet 만들고, NACL 만들고, ACG 만들고.. 많이 해야 한다.<br>
>이런 과정을 샘플코드를 통해 한번에 생성/삭제 다 가능한 실습을 진행해보자.<br>
>1. 루트에 mkdir terraform후 거기에 테라폼 설치함(wget ~~~~.zip -> unzip ~~~~.zip)<br>
>그리고 mv terraform /usr/bin<br>
>그리고 terraform version으로 설치 확인 완료!<br>
>2. 테라폼 예제코드를 다운받아서 사용했음
>>wget https://kr.object.ncloudstorage.com/test001/Terra_20221121.zip<br>
>>unzip Terra_20221121.zip<br>
>>테라폼은 확장자가 .tf이다. 압축 풀면 main.tf, versions.tf, variables.tf가 있다.<br>
>3. 테라폼 검증 (terraform init)
>4. 테라폼 플랜 (terraform plan)
>5. 테리폼 실행 (terraform apply) : 서버 생성되는 거 기다리면, 생성됨!
>6. 테라폼 생성 리소스 삭제 (terraform destroy)
>
>!! 참고<br>
>**Terraform 파일 예제**를 보기 편하게 정리해두었다 
>- [main.tf](https://github.com/yyhh314/TIL/blob/main/Network/NCLOUD/main.tf_content.txt) 
>- [variables.tf](https://github.com/yyhh314/TIL/blob/main/Network/NCLOUD/variables.tf_content.txt)



{: .new-title }
> 2023.02.10 (금) - 네이버 클라우드 특강
>
>[사용한 상품]<br>
>- Compute의 **Load Balancer**<br>
>
>**[LoadBalancer 실습]**<br>
>■ NAVER CLOUD 핵심 서비스로 간단한 웹 애플리케이션 만들기<br>
>ㄴ> "안전성 & 고가용성을 확보한" **by Load Balancer!**<br>
>
>1. **VPC 생성**<br>
>Subnet 생성 (lb, private, public subnet 생성!)<br>
>Network ACL설정
>> lb, private, public nacl을 생성!
>> ICMP, TCP에 대한 inbound와 outbound 규칙을 설정!
>> ex) 웹 접속 할거라서 public nacl의 inbound에는 80포트를 지정했어야 했다. ssh접속도 할 거라서 22포트도 지정했다. 
>> 그리고 저번실습때 사용한 Init Script를 사용하여 웹(httpd)또한 서버에 세팅했다.
>2. **LoadBalancer의 Target Group 생성**<br>
>> 로드밸런서에 이 Target Group을 지정하게 된다.
>> 프로토콜, 포트, Target유형, 연결 로드밸런서, VPC 정보를 볼 수 있다. (HTTP, 80, VPC Server)
>3. **LoadBalancer 생성** (application loadbalancer!!)<br>
>> 대상 vpc를 지정 
>> LoadBalancer subnet을 선택 
>> 리스너를 설정(프로토콜과 포트! http, 80을 설정)<br>
>> Target Group을 선택<br>
>
>**─▶ LoadBalancer 생성 완료!**<br>
>
>웹 접속시 서버 계속 바뀌는 것을 확인했다. 부하분산이 일정하게 되고 있는 모습 봄.<br>
>Auto Scaling Group도 만들어서 Auto Scaling 대상이 되는 서버그룹을 관리해봄. (Target Group을 로드밸런서 타겟으로 지정)<br>
><br>
>아ㅠㅠ 오늘 많이 졸았는데 녹화본도 없어서 좀 어렵고 정리가 안 된다..!<br>
>실습한 게 더 있었는데 혼란스럽네..!?<br>
>로드밸런서 중요한 개념이었는데.. 김예은 반성해야겠다.<br>
>Todo에 적어두고 다음에 또 만나자. <br>
>
>■ NCA 자격증을 인식했다! 기출문제 몇개 풀어봄<br>
>ㄴ> 무료 접수기회 있으니까 한번 해봐??<br>


{: .new-title }
> 2023.02.13 (월) 
>
> - 팀프로젝트
> - nginx


{: .new-title }
> 2023.02.14 (화) 
>
> - Cloud 복습


{: .new-title }
> 2023.02.15 (수) 
>
> - 졸프 : 라디오 포매팅 & 회의
> - Cloud 복습


{: .new-title }
> 2023.02.16 (목) 
>
> 하루종일 놀았다.. 팀원들이랑 밥->카페->보드게임!<br>
> 유은님께 COUP라는 겜을 배웠는데 와 진짜 이거보다 재밌는 보드게임 없다..

{: .new-title }
> 2023.02.17 (금)
>  
> 졸프 미팅 준비 & 조교님과 미팅 => 정말 최고야..


{: .new-title }
> 2023.02.23 (목)
>
> 졸프 : 백엔드 구축 시작 : 기능추가 : mp3 -> DB


{: .new-title }
> 2023.02.27 (월)
> 
>gcp api 사용해서 stt를 진행<br>
>python gui 사용을 위한 세팅


