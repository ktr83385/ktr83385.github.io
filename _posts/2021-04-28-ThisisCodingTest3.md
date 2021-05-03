---
title: "이것이 코딩테스트다 (2)"
excerpt: "이것이 코딩테스트다 (2)"
toc: true
toc_sticky: true
categories:
  - 코딩테스트
tags:
  - Python
  - 나동빈
  - 코테
  - 코딩테스트
last_modified_at : 2021-05-03T20:45:00+05:00
---

https://www.youtube.com/watch?v=m-9pAwq1o3w&list=PLRx0vPvlEmdAghTr5mXQxGpHjWqSz0dgC

**이것이 코딩테스트다 - 나동빈**

강의를 듣고 나서 정리 겸 나중에 복습하기 위해 포스팅합니다!!

# 3,4 . 파이썬 문법 - 수 자료형, 리스트 자료형

---

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/6b2efe71-c121-42a0-b8f6-74f50ae988f2.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=1888.4252488207092)


어떤 프로그래밍을 작성하던 간에 <span style="color:blue">자료형</span>을 활용해야 하기 때문에 **자료형에 대한 이해**는 필수적이다. **파이썬에서는 자료형의 기능이 다양하고 강력**하므로, **다양한 알고리즘을 작성할 수 있다.**

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/8cc33b7c-1b05-419c-a4f5-e2623b00d8bc.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=2184.784455053406)


\-0.7 이라면 0을 생략하고 -.7 이라고 표현할 수 있다. 또한 소수부가 0일 때 또한 0을 생략할 수 있다. ex) 5.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/31c477e5-3431-4b11-be58-63a2ae501b30.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=2195.5000580534056)


**e, E**를 이용해 **지수 표현 방식**도 이용할 수 있다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/b15452f7-1f03-463e-9db6-49ca5529c841.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=2293.235415868393)

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/d06e1a48-934c-4236-a09a-1b6959a0dbf7.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=2365.272891026703)


4바이트 혹은 8바이트의 고정된 크기의 메모리를 할당받기 때문에, **고정된 크기의 메모리를 할당한다는 점**에서 이러한 실수 정보를 표현하는 **정확도 측면에서 한계**를 가질 수 밖에 없다. 예를들어 일상생활에서 자주 사용하는 **10진수 체계**에서는 0.3과 0.6을 더한 값이 0.9로 정확히 떨어진다. **하지만 2진수에서는** 0.9라는 값을 정확하게 표현할 방법이 ~~없다~~. 따라서 컴퓨터는 0.9와 가까이 표현하지만, 미세한 오차가 있을 수 밖에 없다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/6570421f-5871-4f71-b012-df28edc1815d.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=2435.3743040419618)


a 가 0.9가 아니라고, False값을 반환하는 것을 알 수 있다. 이러한 **표현상의 한계를 극복하기 위해 어떤 방법을 사용할 수 있을까?**

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/30911089-549e-4fdd-a785-287bfc8c5dd1.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=2466.998822041962)


이럴 때는 round() 함수를 이용할 수 있다. 반올림 목적으로 사용할 수 있다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/e04f1835-49ea-48c4-a8b6-00e40271587a.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=2507.991998927521)


round()함수를 사용했을 때 True를 반환하는 것을 볼 수 있다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/0a419658-e8ba-4ecb-b757-af76691be00a.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=2523.509422929428)


파이썬에서는 **나누기**를 수행할 때 나눠진 **결과를 실수형으로 반환한다.** 또한 몫 연산자로는 **"//"**를 사용한다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/7f0d2a8b-1581-4a7c-8fca-37f3fd78c21f.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=2602.6757619809264)


나누기를 수행했을 때 실수형으로 나오고, 나머지와 몫을 구할 수 있다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/a8871087-9ed7-46b4-9f11-1afbacf3f756.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=2625.404635)


거듭제곱 연산자(\*\*)도 사용이 가능하다

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/dafcf20c-5bd7-41d7-8949-07650cfd9a5a.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=2633.5777068588563)


<span style="color:blue">리스트 자료형</span>은 데이터를 연속적으로 담아 처리하기 위한 자료형이다. C와 Java에서의 배열의 기능을 제공한다고 볼 수 있고, 그와 더불어 연결리스트와 유사한 기능을 지원한다고도 이해할 수 있다. 파이썬의 리스트 자료형은 연속적인 데이터가 메모리에 올라가 있을 때, 반복적으로 그 뒤 쪽에 데이터를 이어 붙힐 수 있는 <span style="color:blue">append</span> 함수를 제공하고, 또한 뒤쪽에서 데이터를 제거하는 기능 등도 제공한다. 따라서 일반적인 배열과 비교했을 때, 더욱 다양하고 유용한 기능들을 제공한다는 점이 특징이다. 자바에서의 ArrayList와 비슷하다. 또한 List 자료형은 여러개의 유사한 성질을 가지는 데이터가 연속적으로 담겨야 할 때 많이 사용한다는 점에서 테이블이라고 부르기도 하고, 그냥 배열로서 쓸 때는 배열이라고 부르기도 한다. 기본적으로 리스트를 이용하면 되겠구나라고 이해하면 되겠다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/54907eb0-f537-4110-8ce1-a8f94704dbde.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=2727.188471017166)

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/e5d02942-7cbd-4856-95be-5acfb2a12e49.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=2770.4624001125335)


1부터 9까지 연속적인 데이터를 담는 a를 초기화 한 것을 볼 수 있다. 또한 파이썬에서는 특정한 크기의 리스트를 임의의 값을 넣어서 초기화할 수 있다. 이렇게 모든 값이 0인 길이가 10인 리스트를 초기화하고자 한다면 이런식으로 코드를 작성할 수 있다. 값으로 0을 담고 있는 크기가 1인 리스트를 총 10번 곱해서 쭉 옆으로 늘어뜨린다고 보면 되겠다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/07edc701-9489-4626-9c64-d66626e1f156.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=2911.208239034332)


정식 명칭은 인덱싱이다. 양의 정수, 음의 정수 모두 사용 가능하다. 한 가지 유의할 점은 음의 정수를 사용한다면 -1부터 시작한다는 것이다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/8927f95e-7a5e-4285-88cc-698f71630d73.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=2946.5276920095366)


앞에서 8번 째 원소는 a\[7\]이지만, 뒤에서 첫 번째 원소는 a\[-1\]임을 볼 수 있다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/7dce6f68-bbeb-4d9d-87bb-804d57e92bb0.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=2978.612888213623)


파이썬은 슬라이싱을 제공한다는 점에서 매우 유용하게 연속적인 데이터들을 한꺼번에 가져올 수 있다. 이때 참고해야할 점은 끝 인덱스는 실제 인덱스보다 1을 더 크게 설정해야한다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/c3db9da4-4dcf-4e5f-9ded-ecdc8ca7d298.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=3029.389664973297)


4번째 원소까지 가져오고 싶을 때 :4 인것을 볼 수 있다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/99451542-f8c5-4e4e-af57-1c690ca7b46a.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=3076.4748668149873)


리스트 컴프리헨션은 파이썬이 제공하는 또다른 강력한 기능 중 하나이다. 대괄호 안에 조건문과 반복문을 적용하여 리스트를 초기화하는 구문을 매우 간결하게 작성할 수 있다는 점이 그 특징이다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/cc11cb79-1635-49f9-8255-08186022906a.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=3123.810580125885)


0부터 9까지 매번 증가를 하면서 반복을 할 때마다, i의 값들을 원소로 설정해서 리스트를 만들겠다는 거다. range(10)은 0부터 9까지 값들을 차례대로 i가 순회할 수 있도록 만들어준다. 단 한 줄만에 우리가 원하는 방식으로 원소를 리스트에 삽입해서 한 번에 초기화할 수 있는 것을 확인할 수 있다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/2646bc8d-154c-4ca0-99e0-3ce61fec75dc.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=3206.5567241029967)


리스트 컴프리헨션을 이용하게 되면, 원래는 더 길게 작성해야하는 코드를 간결하고 짧게 작성할 수 있다는 점이 장점이라고 할 수 있다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/4f407cce-b2af-4f38-a860-0c112c1075eb.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=3215.1568390305174)


조건문까지 포함할 수 있다. i가 0부터 19까지 반복을 하되, 그 때 그 i가 2로 나눈 나머지 값이 1인 경우에만 그 원소인 i로 리스트를 만들겠다라고 하면 위처럼 작성할 수 있다. 정수가 홀수일때만 리스트에 담겠다와 같은 의미이다.


또 다른 예시로 1부터 9까지 제곱 값을 포함하는 리스트를 만들고자 한다면 매번 i \* i 를 그 원소로 설정할 수 있다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/297453ec-2540-4ba2-820b-3c0947bbc76c.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=3278.5238241735688)


리스트 컴프리헨션을 이용하게 되면 원래는 4줄 이상의 코드를 1줄로 대체할 수 있다는 것이다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/777cdf66-d92e-4b2a-a2bc-ee41336c636f.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=3309.356645994278)


또한 2차원 리스트를 초기화할 때 효과적으로 사용될 수 있다. 특히 이렇게 다양한 코테 문제에서는 N \* M 크기를 사용해야할 때가 많다. 왜냐면 문제 상황 자체를 N \* M 크기의 맵 상에서 벌어지는 상황으로 정의하는 경우가 많기 때문이다. 그때 리스트 컴프리헨션을 사용한다면 간단하게 2차원 리스트를 초기화할 수 있다.

다만 이 때 유의할 점이 있는데, 2차원 리스트를 초기화 할 때 array = \[\[0\] \* m\] \* n같이 작성하게 되면, 예기치 못한 결과를 초래할 수 있다. 그래서 일반적으로 2차원 리스트를 만들 때 이렇게 만들면 잘못된 예시라고 볼 수 있다. 

파이썬은 기본적으로 리스트 자료형을 이해해서 어떠한 변수값을 할당하게 되면 내부적으로 그 리스트는 객체 형태로서 처리가 되고, 별도의 주소값을 가지게 된다. 따라서 단순히 이렇게 리스트 객체 자체를 n번 곱하도록 만들게 되면 단순하게 내부적인 길이가 m인 리스트를 그냥 n번만큼 그 참조값을 복사하는 것과 같기 때문에 이 경우는 내부적으로 포함되어 있는 이 리스트가 모두 동일한 객체, 즉 같은 객체로서 인식된다는 특징이 있다. 

다시 말해, 이렇게 만약 2차원 리스트를 초기화하게 된다면 내부적인 리스트는 모두 같은 리스트로서 처리가 되기 때문에, 내부 리스트 중에서 특정 위치의 하나의 값만 바꾼다고 하더라도, 모든 리스트에 그 변경사항이 적용되기 때문에 예기치 못한 결과가 나올 수 있다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/ae31047f-415c-4db9-bee7-6d2cb0a40839.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=3441.437875032425)


먼저 좋은 예시이다. n번 반복을 할때마다, 길이가 m인 리스트를 매번 초기화해서 이 전체 2차원 리스트를 특정한 변수에 대입해주면 되는 것이다. 이 경우에는 특정 위치의 값을 바꾼다면 그 위치만 정상적으로 변경이 된다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/e3733318-b60e-4797-b34a-e037490a31b7.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=3488.1338779771118)


만약 이런식으로 2차원 리스트를 초기화하게 되면, 어떻게 되냐면 전부다 0으로 초기화 된 것으로 보이지만, 특정한 위치의 값을 바꾸게 되면, 원래 우리가 바꾸고자 하는 값은 \[1\]\[1\]인데, 바뀐 결과를 확인해보면 모든 내부 리스트에서 값이 바뀐 걸 확인할 수 있다. 이처럼 이러한 방식으로 2차원리스트를 초기화하게 되면 내부적인 리스트가 모두 같은 개체로서 인식될 수 있다는 점을 유의하면 된다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/8b5f5005-d184-4ce8-af7c-f6b79a0aa36e.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=3524.9583499408723)


언더바를 언제 사용할까? 반복을 사용하되, 반복을 위한 변수의 값을 무시하고자 할 때 언더바를 자주 사용한다. i의 경우 i의 값을 계속해서 더해가는 코드이므로 이렇게 변수명 i를 넣어준 것이고, 만약 내부적으로 변수값이 사용되지 않고 단순히 내부적으로 어떤 작업을 반복하고자 한다면 언더바 처리를 해서 넘겨줄 수 있다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/d236931a-e6dd-4b36-ac30-c3f801dbe8d2.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=3591.6508651773834)


리스트 관련 함수들로는 이런 것들이 있다. 코테에서 많이 사용되는 함수 위주이다. 

append()는 가장 뒤쪽에 하나의 원소를 새롭게 추가하기 때문에 시간복잡도는 상수시간이다. 

또한 별도로 sort()함수를 사용하면 리스트가 내부적으로 가지고 있는 변수들을 자동으로 정렬하게 된다. 내림차순으로 정렬 또한 가능하다. NlogN의 시간복잡도를 가진다. 

이어서 모든 원소의 순서를 뒤집을 땐 reverse(), 

특정한 인덱스 위치에 원소를 넣고자 할 때는 insert(), 

특정한 값을 가지는 데이터의 개수를 구할 때는 count(), 

특정한 값을 가지는 원소를 제거할 때는 remove를 사용할 수 있다. remove()함수는 특정한 값을 가지는 원소가 여러개라면, 하나만 제거한다는 점이 특징이다.

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/e98eadb1-164c-4d3d-8dab-ff5f8166fbd1.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=3693.0084848493193)

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/70848b2e-ac14-46b6-8223-41067e734f53.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=3714.4618340839233)

[![이것이 코딩테스트다 (3)(4) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/765ec8bdfa06462187c5147701ecc4c4/f954ed76-4488-447b-bec2-aaceb2793c23.png)](https://slid.cc/vdocs/765ec8bdfa06462187c5147701ecc4c4?v=3681bf126a39475b9871422e8573cdca&start=3752.983645020981)


리스트에서 특정 값을 가지는 원소를 모두 제거하고자 한다면 어떻게 해야할까? remove()함수는 하나의 원소만 제거해준다. 따라서 모두 제거하고자 한다면 위와 같은 방식으로 코드를 작성할 수 있다.이 때, 집합 자료형을 사용할 수 있다. 집합 자료형은 특정한 원소의 존재 유무만을 체크하고자 할 때, 매우 효과적으로 사용될 수 있는 자료형 중 하나이다. a라는 리스트를 i라는 변수가 하나씩 확인 하면서 i라는 변수가 remove\_set에 포함되지 않다면 그 때의 그 원소만을 남겨두겠다는 것이다.
