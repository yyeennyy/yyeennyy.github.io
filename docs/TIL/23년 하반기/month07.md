---
title: 2023년 7월
layout: default
grand_parent: TIL
parent: 23년 하반기
nav_order: 2
---

#### 이번달 집중할 것 : 코테랑 졸프, 그리고 새로운 프로젝트
<br>

{: .new-title }
> 2023.07.03 (월)
> 
> 1. **맥OS의 .DS_Store파일**<br>
> - 맥 시스템이 finder로 폴더에 접근할 때 자동으로 생김
> - 해당 폴더에 대한 메타데이터를 저장
> - os.listdir로 특정 디렉토리에 존재하는 파일을 불러오는 과정에서 발견했음. 그래서 제외해줌.
> 
> 2. **다글로 서비스**
> - whisper보다 개선된 STT모델을 연구개발 성공한 '다글로'를 알게 됨 → 1시간짜리 wav를 2분30초 내로 STT완료 & 정말 멋진 결과물이다.. 졸프 분발해야겠다


{: .new-title }
> 2023.07.08 (토)
> 
> 1. **Toss Next 코테**를 보면서 현황을 반성함
> 


{: .new-title }
> 2023.07.12 (수)
> 
> 1. **코테 - BFS**<br>
> 전형적인 BFS 문제들이 쉬워졌다. 익혔음!
>
> 2. **정처기 실기** 공부 시작! 10일 남았다.
> 

{: .new-title }
> 2023.07.13 (목)
> 
> 1. **코테 - BFS**<br>
> q에 중복 값을 안넣기! 확실히 인지함 (시간초과) 
> 
> 2. **HashMap, KeySet, Iterator**<br>
> HashMap에서 keySet()을 뽑아 iterator()를 통해 Iterator객체를 얻었다.
> for문에서 쓰기보다는 while문에서 hasNext()와 next()를 통해 다룬다.


{: .new-title }
> 2023.07.24 (월)
> 1. **음성 데이터 특징**<br>
> "광고/노래 음성 분류기"를 제작해야 한다. (졸프)<br>
> 다양한 음성 특징을 기반으로 학습 데이터 생성에 노력했다.<br>
>   - Spectral Centroid<br>
>   - MFCCs<br>
>   특히 위 두개에 관심이 갔다.<br>


{: .new-title }
> 2023.07.25 (화)
> 
> 1. **디자인패턴 - 싱글톤**<br>
> - 가장 단순 방법은 private 생성자를 두고, 인스턴스 생성 메서드에서 null 체크하는거. 당연히 thread-safe하지 않음.
> - thread-safe하게 만들기 위해 또 단순히 생각해보자면 synchronized 키워드를 사용할 수도 있겠지. 하지만 이것은 성능에 부하가 큼.
> - static Singleton instance를 '미리 초기화'하는 방법. 그치만 만약 이 인스턴스가 생성 비용이 아주 크고, 메모리 할당량이 크고, 당장 사용하지 않을 거라면? 낭비! 그리고 필요로 하는 시점에 만들고 싶은데 그러지 못해..
> - 'double checked locking!' synchronized 전후에 null체크를 한번씩 총 두번 하자. 그러면 멀티쓰레드에서 간혹 null안에 동시에 들어오는 상황에서만 (cost가 큰) synchronized 키워드를 사용하게 되고, 그런 멀티쓰레드의 동시접근 상황이 아닌 상황에서는 그냥 null체크로 충분하게 됨! 좀 더 부담이 없겠다. (이때, volatile을 이해해야 한다. 꽤나 복잡한 이야기. 공부하자.)
> - 레이지로딩! 권장하는 방법 중 하나이다. static inner class를 두는 방법! 그리고 이 inner class 안에서 new하면 된다. thread-safe하며, lazy loading도 가능하고, 복잡한 이론적 배경도 없음.
>
> 지금 이 모든 방법은, 깨뜨릴 수 있는 다양한 코딩 방법들이 존재한다.  


{: .new-title }
> 2023.07.26 (수)
> 
> 1. **졸프 - 음성 데이터 기반 Classifier**<br>
> 광고/노래 음성 분류기를 만들고 있었는데 확실히 만드려고 다시 자료조사에 나섰다. 오늘 배운 것은?<br>
> --> SOTA 모델 찾는 방법을 배움 : [Browse State-of-the-Art](https://paperswithcode.com/sota) 이 사이트에서 찾기 좋다<br>
> --> 많은 공부가 된 관련 프로젝트 발견 : [(링크)](https://hajunyoo.oopy.io/projects/audio-alert-latefusion-project) 여기에서 많은 배경지식을 얻음! (피처 엔지니어링, fine tuning, early/late fusion(특히 early), 스펙트로그램 분류에 있어서 Densenet의 장점 등)
> 
> 2. **코테 - greedy**<br>
> 오늘 BOJ2457공주님의정원 진지하게 풀었다. 어제 공부한거 적용하기 좋은 문제!<br> 
> --> 301~1101 날짜 범위니까 기껏해야 O(276N)이라는 것을 보았으면 좋았겠다.<br>
> --> 결국 모든 t가 포함되어야하니까 t를 꽃이지는시간max만큼 늘려가면서 체크하면 깔끔했다.<br>
> --> 꽃리스트를 굳이 내림차로 하고 꽃삭제하고 갱신하고 안해도 됐었다. 그래도 차분히 생각해서 올바른 알고리즘 만든 것은 칭찬!


{: .new-title }
> 2023.07.27 (목)
>
> 1. **샘플링**<br>
> 원래 다양한 wav를 샘플링하지 않고 사용했다.<br>
> 그러나 확실히 해두는 것이 좋다고 생각하여 22050Hz로 통일했다.<br>
> 
> 2. **early fusion**<br>
> 어제 알게된 early fusion을 통해 피처 준비를 해보았다. <br>
> --> 세개의 스펙트로그램 이미지(stft, mfcc, melspectogram)를 이어붙임<br>
> --> Encoder Model을 통과시켜 피처를 얻음 (애매하다!)<br>
> 올바른 방법은 모르지만, 간단히 진행해보았다.<br>
> 
> 3. **Densenet**<br>
> pretrained model인 Densenet121을 통하여 32x32x3 인풋 데이터에 대한 분류기를 만들었다. 그런데 분류를 전혀 하지 못하더라고!(심지어 이진 분류임)<br>
> 뭘 모르고 잘못 만든듯! 내일 정정해야겠다. 




{: .new-title }
> 2023.07.28 (금)
>
> 1. **특정 파일만 이전 커밋으로 돌리기 (checkout)**<br>
> [블로그에 기록함](https://splendidlolli.tistory.com/624)<br>
> checkout은 브랜치 이동만 하는 게 아니고, 특정 커밋으로 변경할 수도 있음을 배웠다.<br> 즉 **git checkout 브랜치명** 뿐만 아니라 **git checkout 커밋ID**할 수 있다.<br>
> 팀원이 푸시한 split_module가 돌아가지 않았고, 이전 모듈이 잘 작동되었기 때문에 문제의 split_module만 이전 커밋으로 돌려서 개발을 진행했다.
>
> 2. **어제 Densenet 모델이 이상했던 원인: 오타**<br>
> ad데이터랑 music데이터를 섞어야 하는데 ad데이터랑 ad데이터를 섞는 오타를 냈다.<br>
> 수정해서 다시 Densenet Classifier 결과 확인! 와.. 너무 좋은데?<br>
> --> Test Accuracy: 1.0<br>
> --> Loss: 0.008<br>
> 그러나 실전 데이터셋에 테스트해보니까 좋지 않았다. <br>
> 
> 3. **피처사이즈를 키워 분류모델을 개선했다**<br>
> ▶ 스펙트로그램 size:<br>
> &nbsp;&nbsp;&nbsp;&nbsp;- 전: 64x64*3<br>
> &nbsp;&nbsp;&nbsp;&nbsp;- 후: 256x256*3<br>
> ▶ 인코딩 후 피처 size:<br>
> &nbsp;&nbsp;&nbsp;&nbsp;- 전: 32x32x3<br>
> &nbsp;&nbsp;&nbsp;&nbsp;- 후: 128*128*3<br>
> 개선이 되었다.<br>
> 과정 정리: 

{: .new-title }
> 2023.07.29 (토)
> 
> 1. **분류기 개선**<br>
> 2. **졸프회의**<br>


{: .new-title }
> 2023.07.30 (일)
> 
> 1. **디자인패턴 - 프록시**<br>
> 사용하려는 클래스를 직접 갖다쓰는게 아니라 프록시(대리인)을 거쳐서 사용<br>
> 즉 요청은 프록시가 받음! <br>
> <br>
> - **기본 구조**<br>
>   - 프록시는 실제객체를 참조할 필드가 하나 필요! (즉 실제객체의 인터페이스타입이 필드를 둔다)<br>
>   - 인터페이스를 implement하면서, 사용할 기능을 overriding하여, 부가로 필요한 기능을 추가하면 된다
> <br> 
> - **기능 예시**
>   - 객체원본코드를 건드리지않고 **연산수행시간을 측정**하고 싶다면? 메서드 A를 overriding하여, overriding한 A안에서 실제객체의 A를 부르고 그 앞뒤로 타임체킹 코드를 넣을 수 O<br>
>   - **초기화 지연**도 마찬가지다!<br>
>   - 손쉽게 **원하는 기능을 기존코드 건드리지 않고 추가가능**하다.<br>
>   - 그럼 당연히 **로깅**도 추가할 수 있고<br>
>   - **캐싱**도 추가 가능! (사용하려는 메서드가 리턴타입이 있다면, 캐싱을 도입해 볼 수 있겠지!)<br>
>   - 즉 프록시는 캐싱처럼 성능적인 이점을 가져올 수 있다. <br>
><br>
> 
> **그래서 OCP원칙을 준수하려는 패턴이며<br>
> 또한 자연스레 SRP도 지키게 된다<br>**


{: .new-title }
> 2023.07.31 (월)
> 
> 1. **광고/노래 분류기 완성!**<br>
> 공부좀 더 했더니 좋은 분류기가 탄생했다.<br>
> - 보완함<br>
>   - **이미지 사이즈**<br>
> 다운샘플링시에는 영역보간법이 효과적이다(cv2.INTER_AREA)<br>
> 스펙트로그램 사이즈는 (224, 224)로 조정했다.<br>
> 사용할 pretrained model의 default input이기 때문.<br>
>   - **피처 개선**<br>
> 팀회의 이후 early fusion이 불필요하다는 의견 수용<br>
>   → 개선 전: 불분명한 피처 + 의미없는 채널<br>
>   → 개선 후: 3종의 스펙트로그램 데이터를 각 채널로 두고 model에 바로 넣음<br>
>   - **스펙트로그램 이미지 RGB**<br>
>       RGB는 의미 없다! (그냥 수치의 컬러맵)<br>
> - 진행함<br>
>   - **그리드서치**<br>
>   - **Classifier: Densenet121과 Resnet50을 비교**<br>
> - 결과 : 나름 대만족<br>
> [**▶ 최종 ipynb 바로가기 ◀**](https://colab.research.google.com/drive/1rP-6Kyf6bo3XEGKDx6gHTnu7XczNDuPI)