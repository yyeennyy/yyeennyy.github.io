---
title: 2023년 4월
layout: default
grand_parent: TIL
parent: 23년 상반기
nav_order: 4
---


{: .new-title }
> 2023.04.04 (화)
>
>1. **교수님과 회식**<br>
>그리고 이번 데이터통신 과목에서 교수님이 샤잠 알고리즘 한번더 설명해주셔서 감사했다.


{: .new-title }
> 2023.04.10 (월)
>1. **블록코딩, 라인코딩 이론**<br>
>복습겸 적어보자면.. 
>라인코딩은 디지털 1bit를 만들어내는 것. 즉 
>라인코딩은 한순간의 정보를 단 한 개씩 보낸다. 단점 첫번째는, 오류정정이 불가하다는 것. 단점 두번째는, 느리다는 것. 그래서 대안이 블록코딩 방식이다. 빠르고, 오류수정 가능하다. 자세한 내용은 따로 공부!
>
>2. **졸프 V1 고민**


{: .new-title }
> 2023.04.14 (금)
> 
>shazam / finding peak points 이해<br>
>졸프 : 조교님 미팅

{: .new-title }
> 2023.04.17 (월)
> 
>**데이터통신 과제** : 사인파 함수를 주파수 함수로 변환한다. 그리고 오디오의 어떤 영역에서 가장 큰 주파수를 찾아내는 코드를 작성했다. 좀 생략하여 간단 코드를 첨부해보자면..<br>
>- ftt를 통해 주파수 스펙트럼을 얻는다.<br>
>spectrum = scipy.fftpack.fft(audio)<br>
>- 이 결과는 복소수값이다. 절댓값처리하여 진폭정보만 남기자.<br>
>spectrum = np.abs(spectrum)<br>
>- 가장 큰 진폭을 가지는 주파수를 얻는다.<br>
>top = np.argmax(spectrum)<br>
>- 근데 이 top값은 실제 주파수가 아님을 유의해야 한다.<br>
>top = top * samplerate / len(audio)



{: .new-title }
> 2023.04.20 (화)
>
>큐넷 기사시험 원서접수 매크로 만들었다 <br>
>(제작동기: 나도 좀 늦게 신청해서 죄다 마감되어서 깜놀)<br>
>- 일단 결제방법 선택 전까지 동작함
>- 대기큐 처리는 아직 X
>- 다 마감찼는데 가끔 취소되는 자리 줍줍할때 매우 용이함
>- 희망(가능) 날짜와 지역을 입력하면 줍줍해준다
>- gui 없음!