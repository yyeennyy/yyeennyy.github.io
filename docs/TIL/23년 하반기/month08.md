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
>
> 3. **git - revert와 reset**<br>
> - revert: 되돌렸다는 커밋기록을 남기며 되돌리므로, 이미 원격지에 push한 뒤라면 revert가 적절함<br>
> - reset: 커밋 자체를 삭제하므로, 원격지에 push한 뒤라라면 함부로 reset하면 안됨<br>
>   - 필요시 로컬에서만 사용하자.



{: .new-title }
> 2023.08.02 (화)
> 
> 1. **스펙트로그램 정규화**<br>
> [블로그 기록: 스펙트로그램 정규화 필요성 (음성처리)](https://splendidlolli.tistory.com/626)<br>
> ✨ STFT:  np.log(1 + 1000 * np.abs(stft))<br>
> ✨ MFCC: min-max<br>
> ✨ Mel spectrogram: dB로 변환<br>
> 적절한 정규화방법을 적용하려 노력했다.<br>
> 

{: .new-title }
> 2023.08.03 (수)
> 
> 1. **분류기 망함!**<br>
> 내생각엔 학습데이터가 너무 모집단을 대표하지 못한 것 같다.<br>
> 반성거리가 있다면, 나는 너무 검토를 대충 하고 실천하는 것 같다는 것이다.<br>
> 이번 일을 기억하며 사전에 고민을 하는 습관을 가지도록 하자.<br>
> 기록도 더욱 습관화하고!<br>



