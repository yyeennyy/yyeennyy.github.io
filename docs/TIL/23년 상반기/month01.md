---
title: 2023년 1월
layout: default
grand_parent: TIL
parent: 23년 상반기
nav_order: 1
---
#### TIL의 시작!
#### **12월 말: SW 아카데미에서 Spring 학습에 집중**

{: .new-title }
> 2022.12.20 (화)
> 1. **코테**<br>
> BFS 응용문제 잘 못풀길래..<br>
> BFS를 연습했다<br>
> 나 일단 이번주 BFS뿌시기 간다..
> 
> 2. **SW아카데미**<br>
>  WAS, RMI, SpringBean, kafka.. 접했다.<br> kafka가 좀 어려웠다. 오와 그래도 'kafka를 사용하는 이유'에 초점 맞춰서 잘 공부하면 중요한 개념들을 얻을 수 있을 것 같다.<br>
> RMI랑 SpringBean도 몇번 다시 읽어보면서 내가 설명할 수 있을 정도로 공부하면 좋겠다.<br>
> Web Server랑 WAS 차이도 공부했다. 사실 예전에 봤던 것들인데, 혼자 공부할 때는 그냥 아그렇구나 하면서 넘어간 부분인데, 강사님께서 강조를 많이 하셔서 다시 찾아가며 공부했다. <br>역시 구멍난 부분이 많았다.


{: .new-title }
> 2022.12.21 (수)
>1. **코테**<br>
>오늘도 BFS!!<br>
>좀 기억해야 할 것... 처리대상 노드는 일단 q에 넣는 거라서 첫시작도 q에 넣고가자는 생각을 합시다 & q size를 현시점에 고정시켴서 일단 쭉 처리하고, 다시 size checking해서 또 q size만큼 쭉 돌고.. 이렇게 끊어서 생각할 줄 알기!<br>
>2. **Figma**<br>
>오늘 figma를 처음 써봤다! 우리 팀 프로토타입을 figma로 만들어야 한다. 너무 좋은 툴 알게되어서 신난다. 일찍 알았음 좋았을텐데! 아무튼 기분좋음! 난 marker 부분을 만들어야 한다.<br>
>우리 팀 파이팅!!<br>
>3. **OS**<br>
>OS가 프로세스 관리하는 거랑 쓰레드.. 공부했다. 지난학기에 OS수업 들었던 게 새록새록.. 많은 CS분야 중 OS는 정말 다시 꼼꼼히 공부하고싶다. 간단히라도 정리해서 이번주 안에 TIL 하나 올려야겠다.<br>


{: .new-title }
> 2022.12.22 (목)
>1. **OS, Memory Management (정리 미완료)**<br>
[링크 : Memory ManageMent](https://github.com/yyhh314/TIL/blob/main/OS/memory_management.md)
>2. **DOCKER 실습**
> Docker실습 하면서 내가 네트워크 지식이 많이 모자라구나 느꼈다. 하긴!! 각잡고 배운 적이 없으니까.. 아무튼 Docker라는 것을 접해봤는데, 중요하다니까 잘 다뤄보고싶다.



{: .new-title }
> 2022.12.23 (금)
> 
>1. **컴포넌트**<br>
>모든 것이 오픈소스는 아니라서 코드재사용한다는 것은 은근 제약이다. 그래서 컴포넌트에 대한 이해가 필요 : 코드없이도 상속, 재활용이 가능하다는 idea<br>
>소스코드없이 컴파일된 결과물을 기반으로 재활용이 가능하다는 것!<br>
>Spring은 컴포넌트 기술 집약체다.<br>
>
>2. **분산컴포넌트**<br>
>그런 재사용을 하려면 원격 호출이 필요 (+ 네트워크 개념)<br>
>(백엔드에서 제일 머리아픈) 분산컴포넌트 기술 등장! '분산'이 들어가면 네트워크 개념이 들어간 것이다. 코드를 원격호출해서 결과를 받아와야 한다든지 그런 개념 등장한 것이다. <br>
>분산컴포넌트를 구현한 것이 MS에서는 DCOM이고 Java에는 EJB 등등.. 근데EJB 다음단계로 Spring Bean으로 분산컴포넌트 기술이 정리됨!<br>
>cf. Spring은 이런 분산컴포넌트 기술에 묘하게 DI를 끌고 들어와서, DI를 반드시 하게 된다. DI는 결국 OOP가 발달한 것이다. 즉 DI는 객체지향.. <br>
>이런 거! 배웠다. 따로 정리하자.
>
>3. **기타등등..**<br>
>결국 궁극적인 스프링 삼각형을 이루려면 POJO가 된다. 스프링은 약간 유사종교성을 가지고 있는데 (<-강사님 말) 궁극적인 열반.. 해탈.. 이것이 POJO인 것임. 참고로 이 수업은 DI까지만 함<br>
>완벽한 객체지향을 위해 DI, AOP로 코드를 짜고, 그렇게 안한(못하는) 것들은 DI로 포장을 하면 된다(=> PSA). 우리가 집중할 80%는 DI다.<br>
>



{: .new-title }
> 2022.12.26 (월)
> 
>1. **Spring 관련 내용을 학습함**<br>
>5달 전쯤에 인프런(김영한선생님) 강의에서 공부했는데, 다시 유사한 내용을 들으니까 더욱 정리가 잘 되어서 좋았다. 핵심부분 정리해서 업로드 완료!<br>
>그나저나 좀 밀렸다. 이거 하루종일 해야 진도 커버 되겠는데..<br>
>SW아카데미에서 살아남으려면 좀 더 부지런해야겠다..!<br>
>2. **네트워크**<br>
>오늘부터 네트워크 수업을 듣는다. 학부에서 아직 안 들은 과목이 네트워크, 데이터통신이라 더 궁금하고 배우고싶다.<br>
>[정리 : OSI 7 layer](https://github.com/yyhh314/TIL/blob/main/Network/OSI_7_layer.md)




{: .new-title }
> 2022.12.27 (화)
> 
>1. **Spring 프로젝트 속성정의파일**<br>
>그동안 Spring 프로젝트의 속성정의파일 application.properties는 그냥 생각없이 쓸거있음 쓰면서 사용하고 있었는데, 오늘 좀 자세히 알게되었다. <br>
>그리고 application context에서 제공하는 주요기능 중 하나인 Environment를 통해 속성관리를 할 수 있음을 알았다. 또한 스프링 환경은 profile과 property를 통해 바뀐다. 그렇다 오늘은 profile과 property 관련 실습을 진행했다.<br><br>
>▼ 스프링 속성을 정의하는 파일
>* **.yaml** <- 요거 가끔 보고 궁금했는데 오늘다뤄봄!
>* **.properties**
>여기에 정의된 속성값들을 꺼내볼 수 있다는 걸 알았다.<br> @Value 를 통해 주입시켜보기도 했다. @Value로 환경변수도 꺼내볼 수 있다는 걸 알고 신기했다!<br>
>또.. Springboot만 지원하는 그런 기능들이 있는데, 기본적으로 실습프로젝트는 Spring 프로젝트다. @Enable어쩌구 이런걸로 Enable시켜서 사용해보기도 했다. 굉장히 다양한 실습을 했고.. 이런게 있구나를 알게되어서 좋다.


{: .new-title }
> 2022.12.28 (수)
> 
> 1. 오늘 하루종일 **ObjectInputStream 관련된 부분 문제해결**했다.<br>
> 블로그에 정리 : [링크](https://splendidlolli.tistory.com/549)<br>


{: .new-title }
> 2022.12.29 (목)
>
> 1. **네트워크 실습 : HTTP srever using TCP socket** <br>
> 간단히 같은 팀원이 띄워둔 서버로 접속해보고, 내 서버로 접속하는 패킷을 캡쳐도 해봤다.
> 2. **Spring logging 실습**<br>
> 와 log file을 이렇게 만들어서 관리할 수 있구나!<br> 나는 다른 개발자분들이 막 운영서버 로그확인해보니까 뭐가 찍혀있다 어떡하냐 이런 말씀 들을때마다 우와 나는 로그확인이라는 걸 언제 해보게 될까? 싶었는데..<br> 개발/운영하면서 이렇게 file로 맘껏 관리할 수 있다는 걸 알고 log랑 좀 친해진 느낌이 든다.
>
> 3. **Selenium 사용해봄**<br>
>진짜 신기했다. 누가 Selenuim 쓰시다가 문제생긴다고 질문하셔서 해결하느라 처음 사용해봤는데 재밌더라!!<br>
>뿌듯한 건 문제 해결도 완전히 해드렸다는 거 ~..<br>
>나중에 직접 써보고 싶다.


{: .new-title }
> 2022.12.30 (금)
>
> **Socket 실습 & TCP/IP** <br>
>지난 학기에 컴프2 들으면서 socket통신을 통한 실시간 채팅 android app 구현 과제를 했던 기억이 났다. 이번에도 그런 실습을 했다. python으로 간단하게! gui 추가하는 부분도 있는데, 일단 하지 않았다. 주말에 후순위로 시간나면 해야지!<br>
개인적인 목표 : Socket통신 프로그램을 다른거 몇개 더 만들어보고, 능숙하게 설명할 줄 알자.<br>
>정리 : [HTTP 통신과 Socket 통신](https://github.com/yyhh314/TIL/blob/main/Network/HTTP_and_Socket.md)
>
> **[DB] Transaction, ACID** <br>
> 야호~~
>[정리 : Transaction_ACID](https://github.com/yyhh314/TIL/blob/main/DB/Transaction_ACID.md)


<br><br>
#### **1월: SW 아카데미와 함께 열공!**


{: .new-title }
> 2023.01.10 (화)
> 1. **spring jdbc 실습** <br>
>반성 : 지난주는 너무 정신없이 지나갔다. 이번주는 다시 원래 텐션 되찾기로 하겠다.


{: .new-title }
> 2023.01.11 (수)
> 
>- [정리1 : mysql 서버 상태 확인하기(show status) │ db connection 전후 Threads 관련 상태변수 확인](https://splendidlolli.tistory.com/560)<br>
>- [정리2 : \[JDBC\] DB Connection 얻어 query 실행 │ DriverManager과 DataSource를 통하여 (+ Connection Pool 개념)](https://splendidlolli.tistory.com/561)
>
>▶ **JDBC와 JDBC driver?**
>- JDBC는 DB를 사용가능케 하는 java의 api이며
>- JDBC driver는 JDBC api가 특정 DBSM에 연결할 수 있게 하는 driver임!<br>DBSM에 따라 적절한 driver를 설치해 사용!
>
>▶ **DB 연결한다는 것은 Connection 객체를 얻는 것임**
>- Connection 객체를 얻는 방법으로 DriverManager, DataSource를 공부!
>- 이때 Connection Pool 개념을 학습하게 됨!
>
>▶ **Connection을 받아온 뒤 query를 날리는 과정을 공부함**
>- connection을 통해 statement를 만들고, statement를 필요에 따라 잘 세팅한 뒤 query를 시행할 수 있음!<br>
>
>▶ **JdbcTemplate**은 편하구나<br>
>- [정리3 : JdbcTemplate │ 왜 Jdbc 'Template'인가? 어떤 동작을 하는가?](https://splendidlolli.tistory.com/563)
>

{: .new-title }
> 2023.01.12 (목)
>1. **NamedParameterJdbcTemplate 실습**<br>
> 쿼리에 값을 전달할 때 ?로 표기되는 placeholder를 사용하지 않고 **이름 기반으로 파라미터를 전달할 수 있게** 기존 코드를 변경해봄<br>
> 순서 말고 키로 매핑되므로 index 실수를 줄일 수 있다. 이때 매핑을 위해 파라미터 Map을 함께 전달했다. <br>
> 실습때 **RowMapper**도 처음 사용해봄. 말그대로 Row Mapper인 것 같다. ResultSet이랑 index가 들어오면 거기 해당하는 객체 반환해주는 Row Mapper! findAll처럼 조회하는 query()에 sql문과 RowMapper를 전달했었음!
> 2. **Spring AOP**<br>
> 이 실습은 여러번 보고 익숙해져야겠다. 덜 소화했다.



{: .new-title }
> 2023.01.13 (금)
> 
> 오늘은 역량평가를 봤는데.. 공부 열심히 해야겠네 김옌...


{: .new-title }
> 2023.01.15 (일)
>
>히루종일 팀개발만 함!<br>
>[글 작성: docker에 띄운 mysql 접속](https://splendidlolli.tistory.com/565)



{: .new-title }
> 2023.01.16 (월)
> 
>오늘도 팀프로젝트에 집중하면서 여러가지를 고민해볼 수 있었음
>
>1. 특정 도메인과 관련된 **여러 Dto를 깔끔하기 관리**하기 위해 static 중첩 클래스 구조를 두는 방식
>2. Dto에 Getter를 둬야지 Json으로 변환될 수 있다는 것 : ResponsEntity가 매핑해주는 과정을 공부하면 된다!<br> [블로그에 정리](https://splendidlolli.tistory.com/566)
>3. 논리적인 **상속 구조를 join 전략**으로 DB에 나타냈었는데, 그래서인지 개발하면서도 계속 DB 설계 관련된 걸 찾아보게되었다. 김영한선생님의 "자바 ORM 표준 JPA 프로그래밍" 이거 공부하고 싶어졌다. 여기 고급 매핑 정보들이 나오는데, 내가 참고한 포스팅들이 다 이걸 기반으로 한 글이더라고..
>
>4. Spring AOP좀 공부+정리해뒀다<br>
[블로그에 정리 : Spring AOP 쉽게 이해하기 | 그리고 간단한 예제코드](https://splendidlolli.tistory.com/567)



{: .new-title }
> 2023.01.17 (화)
> 
> transaction 실습


{: .new-title }
> 2023.01.18 (수)
> 
> web 구조 오버뷰


{: .new-title }
> 2023.01.19 (목)
> 
> 1. 우리가 Springboot를 쓰면 Dispatcher Serlvet, HandlerMapping, HandlerAdapter, ViewResolver 이런 거 다 셋업할 필요가 없다. 그냥 Controller만 작성하면 원하는 결과가 나오기 때문이다. **하지만 너무 자주 사용하고 있는 Controller의 http 요청 처리 흐름을 알고 쓰는 것이 적절한 태도이기 때문에 포스팅해보았다.**<br>
> [블로그에 정리 : Spring MVC | Controller는 어떻게 요청을 처리하는 걸까? | Controller와 Servlet](https://splendidlolli.tistory.com/570)


{: .new-title }
> 2023.01.20 (금)
>
>1. **WebApplicatoinContext**
>- ApplicatonContext 관련된 새로운 개념 인지 : servlet application context & root applicatoin context
>- 여러 개념이 확실히 정돈되지 않음 <br>=> 시간 내서 다시 정리해야겠다. 꽤 복잡하게 느껴졌다. 
>
>2. **REST API**
>- 중요한 것은 "균일한 인터페이스" : **URI로 지정한 리소스에 대한 조작을, 통일되고 한정적인 인터페이스로 수행하는 아키텍처 스타일을 말한다.** 이 아키텍처 스타일이라는 것을 이해하기 어려우니까 "얘가 rest인지 아닌지 말해주는 모델"을 richardson님께서 만드심! maturity model로 설명되었음.<br>
>- REST API를 정말 겉핥기로만 알고 있었는데.. 좀 더 알게된 날이다.
>- 평소에 그냥 **Controller 리턴값**으로 List\<Customer\> 이런식으로 편하게 사용을 했었다. **그럴 수 있었던 이유가 MessageConverter**가 잘 처리해주기 때문이란 걸 알게 됨! 
>
>3. **SPA(Single Page Application)**
>- URL 변경시 **특정영역만 렌더링**된다. DOM 조작을 통한 렌더링이 이루어진다. 단일페이지가 아닌 일반 웹 애플리케이션은 URL 변경시 모든 페이지가 다시 렌더링된다. js, css, layout 등을 다시 서버로 요청하게 된다. (참고: layout 요청시 템플릿엔진을 통함! 아하 그랬던거구나)
>- **SPA 기반 세션관리 <br>└>  확실히는 모르겠음! 공부 필요하다.** 아주 대충 말하자면 : <br>사용자 데이터 모델을 저기 프론트쪽에서 일부 다뤄줄 수 있게 된다. 매번 세션에 정보를 (메뉴정보 등) 넣어주면 세션이 점점 커지는데, 그 사용자데이터모델 일부를 **브라우저의 메모리가 들고 있게 하는 것임.** 그래서 요청을 할 때마다 모델일부에 정보가 담겨있어서, 필요할 때 요청하면 그 메모리에 있는걸 이용해서 처리 가능 (서버에 요청 안하고!) 이렇게 하면 url은 안바뀜. 그래서 html5의 히스토리 api라는 걸 사용하면 url을 바꾸면서 url의 히스토리를 관리할 수 있음! **아무튼 브라우저에서 뷰를 렌더링하는 개념으로 이어짐.**
>- jsp나 타임리프로 보았던 것과는 다르게, **서버에서 처리하지 않고 다이나믹한 렌더링을 처리.. 오키오키..**
>
>4. **CORS**
>- 이건.. 살짝 감을 못 잡았다! 나중에 필요할 때 공부하기로!



{: .new-title }
> 2023.01.24 (화)
> 1. 영속성 컨텍스트
> - 1차 캐시
> - 처리 지연
> 
> **단일 트랜잭션 실습 중 로그를 확인하다가 의문이 생겼고,<br> 결국 영속성 컨텍스트의 '1차캐시' 개념을 이해하게 됨! '처리 지연' 특징까지!**<br>
> [블로그에 정리 : [JPA] Entity는 영속성 컨텍스트에 저장/조회한다!](https://splendidlolli.tistory.com/573)



{: .new-title }
> 2023.01.25 (수)
>1. **H2 db를 사용하며**<br>
>JPA 실습하면서 H2 db를 사용했는데 아직도 이해가지 않는 문제를 만났다.
>- 인메모리니까 스키마 자체가 날아가야 하는 거 아냐?
>- 그리고 crate-drop 설정 했는데 왜 drop이 안돼?<br>
>[블로그에 정리 : [H2] Column이 drop 되지 않음 | 왜 create-drop이 안돼?](https://splendidlolli.tistory.com/576)<br>
>문제 해결은 못했고 임시방편으로 그냥 넘어갔다. 
>
>2. **팀프로젝트 : nginx 이미지 서버 구축 관련 공부**<br>
>아까 2시간정도.. 1팀 모여서 공부했다. 감은 오는데 자세히는 또 모르겠고, 테스트해보려는데 사소한 부분에서 막히고 그랬다. 내일은 더 제대로 공부해보는 걸로 하자. 



{: .new-title }
> 2023.01.26 (목)
>1. **어제 create-drop 설정 안 먹는 문제 해결했다 (바로 다음강의에서 정정해주셨다는...)**<br>
> 테스트에서 JpaProperties를 통해 jpa properties 설정을 가져왔었다. 그런데 **잘못된 설정**에서는 jpa의 바로 아래에 ddl-auto: create-drop 설정을 두었기 때문에 설정을 가져오지 못했던 것이다. JpaProperties를 통해 가져오려면 jpa: 아래에 properties: 아래에 두어야 가능했음!


{: .new-title }
> 2023.01.27 (금)
> 1. 팀프로젝트 - 이미지서버 구축을 위한 **nginx 사용법** 고민 & 적용
> 2. [블로그에 정리: Join 테이블 전략 (상속관계매핑) 상태에서 부모테이블 truncate하기](https://splendidlolli.tistory.com/578)


{: .new-title }
> 2023.01.31 (화)
> 
> jpa transaction에 대한 이해