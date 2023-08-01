---
title: 2023년 8월
layout: default
grand_parent: TIL
parent: 23년 하반기
nav_order: 3
---

#### 벌써 8월 : 코테랑 졸프, 무엇보다도 Spring
<br>


{: .new-title }
> 2023.08.01 (월)
> 
> 1. **버전 충돌 해결**<br>
> (반나절 붙잡은 보람이 있다)<br>
> python의 spleeter모듈 도입은 **크나큰 버전 충돌**을 일으켰다.<br>
> 충돌을 없애고 컨테이너가 정상적으로 올라간 것 같아도, 실제 사용 시점에 not found 문제가 많이 터지기도 하고.. 그치만 해결했쥐!!<br>
> flask, click, black, flask-sqlalchemy, SQLAlchemy, pydub 등 정말 많은 시도와 검토를 반복 했다.<br>
> 버전 충돌을 해결하며 **pipdeptree** 툴을 처음 사용해봤다. 신기하고 편했다!!<br>
> 
> 2. **Dockerfile 간소화**<br>
> 지금까지는 flask 설치 후 뽑아낸 requirement.txt를 전부 Dockerfile에서 설치했다.<br>
> 큰 인식 없이 그냥 했었는데, 사실 pip install flask만 있으면 충분하므로 아예 없앴다.


