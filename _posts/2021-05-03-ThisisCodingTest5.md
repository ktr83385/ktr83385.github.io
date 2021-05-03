---
title: "이것이 코딩테스트다 (3)"
excerpt: "이것이 코딩테스트다 (3)"
toc: true
toc_sticky: true
categories:
  - 코딩테스트
tags:
  - Python
  - 나동빈
  - 코테
  - 코딩테스트
last_modified_at : 2021-05-03T21:00:00+05:00
---


https://www.youtube.com/watch?v=m-9pAwq1o3w&list=PLRx0vPvlEmdAghTr5mXQxGpHjWqSz0dgC

**이것이 코딩테스트다 - 나동빈**

강의를 듣고 나서 정리 겸 나중에 복습하기 위해 포스팅합니다!!

---

# 사전, 집합 자료형

[![이것이 코딩테스트다 (6) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/113ad430f76e45319e6e6718db091ff8/c5d5fdce-2721-427f-8af9-6f9c044d77a3.png)](https://slid.cc/vdocs/113ad430f76e45319e6e6718db091ff8?v=83ea4d1b0e55461b870fa6ba948eba29&start=4284.946300959946)


리스트, 튜플이 값을 순차적으로 저장하는 것과는 대비된다. <span style="color:yellow">리스트</span> 같은 경우는 앞에서부터 뒤쪽까지 차례대로 저장되어있기 때문에 원소 접근에 **인덱싱**을 이용할 수 있었지만, 반면 <span style="color:blue">사전 자료형</span>은 **키, 값** 쌍을 데이터로 가지며 임의의 변경 불가능한 자료형을 키로 사용할 수 있다는 점이 특징이다. 키 값을 이용해서 각 원소에 접근할 수 있다. 또한 해시 테이블을 이용하기 때문에 데이터 조회, 수정에 있어 **상수시간**에 처리할 수 있다는 장점이 있다.

[![이것이 코딩테스트다 (6) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/113ad430f76e45319e6e6718db091ff8/59f176d7-aac4-4665-9c34-edca64eeed55.png)](https://slid.cc/vdocs/113ad430f76e45319e6e6718db091ff8?v=83ea4d1b0e55461b870fa6ba948eba29&start=4328.2974158703)


말그대로 사전과 같이 어떠한 키 값으로 접근을 했을 때, 그것과 매칭되는 어떠한 값을 얻고자 하는 자료구조에서 효과적으로 사용될 수 있다. 

**이처럼 사전 자료형은 특정한 키가 존재하는지 검사하기 위해서 상수시간이 소요되기 때문에** 문자와 같은 키를 이용해서 데이터를 **저장**하고, **관리**하고자 하는 상황에서는 리스트보다 **훨씬 효율적으로** 데이터의 조회를 훨씬 빠르게 수행할 수 있다.

[![이것이 코딩테스트다 (6) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/113ad430f76e45319e6e6718db091ff8/cd7806a0-07f4-4920-ab6a-36b9d94809e4.png)](https://slid.cc/vdocs/113ad430f76e45319e6e6718db091ff8?v=83ea4d1b0e55461b870fa6ba948eba29&start=4438.138181912262)


또한 사전 자료형에서는 키와 값을 별도로 뽑아내기 위해 메소드를 지원한다. 만약 하나의 사전자료형이 있으면 거기에서 **키 데이터**만 뽑고자 한다면 **keys()**함수, **값 데이터**만 뽑고자 하면 **values()**함수.

[![이것이 코딩테스트다 (6) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/113ad430f76e45319e6e6718db091ff8/70fc29b5-5d01-4d43-8259-ae5459d98cef.png)](https://slid.cc/vdocs/113ad430f76e45319e6e6718db091ff8?v=83ea4d1b0e55461b870fa6ba948eba29&start=4457.82316906485)


각 키를 하나씩 출력하고자 한다면 각각의 키값을 출력하도록 만들어줄 수도 있다.

[![이것이 코딩테스트다 (6) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/113ad430f76e45319e6e6718db091ff8/d74eb8af-e4d3-416d-9e1b-555b3b7d596d.png)](https://slid.cc/vdocs/113ad430f76e45319e6e6718db091ff8?v=83ea4d1b0e55461b870fa6ba948eba29&start=4531.742999969482)


엄밀히 말하면 키 함수는 사전 키라는 하나의 객체로서 발현되기 때문에 실제로는 **list함수를 이용해서 list형 데이터로 형 변환을 수행**해주면

[![이것이 코딩테스트다 (6) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/113ad430f76e45319e6e6718db091ff8/9837675d-1838-46df-afd0-7e8500ea0eb2.png)](https://slid.cc/vdocs/113ad430f76e45319e6e6718db091ff8?v=83ea4d1b0e55461b870fa6ba948eba29&start=4545.995574)


정상적으로 **리스트 형태로 출력**되는 것을 확인할 수 있다.

[![이것이 코딩테스트다 (6) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/113ad430f76e45319e6e6718db091ff8/691c5124-bd2d-46ca-992b-fde5cac5ee78.png)](https://slid.cc/vdocs/113ad430f76e45319e6e6718db091ff8?v=83ea4d1b0e55461b870fa6ba948eba29&start=4572.806394146866)


**집합은 중복을 허용하지 않고, 순서가 없다.** 이러한 특징 때문에 집합 자료형을 어떤 데이터가 **존재하는지,아닌지만을 체크**할 때 효과적으로 사용할 수 있다. 또한 **데이터 조회, 수정에 있어서 상수시간**에 처리할 수 있다는 특징도 있다.

[![이것이 코딩테스트다 (6) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/113ad430f76e45319e6e6718db091ff8/16b9accf-bac2-4944-a213-b520b2db2f4a.png)](https://slid.cc/vdocs/113ad430f76e45319e6e6718db091ff8?v=83ea4d1b0e55461b870fa6ba948eba29&start=4612.696013091553)


하나의 리스트가 있을 때, set함수로 감싸주면 집합 자료형으로 초기화할 수 있고, 출력값을 보면 중복이 제거된 상태로 나타나는 것을 확인할 수 있다. 또한 중괄호에 원소를 넣어줌으로써 초기화할 수도 있다.

[![이것이 코딩테스트다 (6) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/113ad430f76e45319e6e6718db091ff8/d95fe5d8-09f5-46f5-be03-9440f02dac1f.png)](https://slid.cc/vdocs/113ad430f76e45319e6e6718db091ff8?v=83ea4d1b0e55461b870fa6ba948eba29&start=4649.412432847412)


집합이기 때문에 합집합, 교집합, 차집합이라는 집합 연산도 제공한다.

[![이것이 코딩테스트다 (6) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/113ad430f76e45319e6e6718db091ff8/58f7287f-e381-455b-96e0-4343852ed448.png)](https://slid.cc/vdocs/113ad430f76e45319e6e6718db091ff8?v=83ea4d1b0e55461b870fa6ba948eba29&start=4678.129342019073)


합집합 " | " , 교집합 "&", 차집합 "-" 을 사용한다.

[![이것이 코딩테스트다 (6) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/113ad430f76e45319e6e6718db091ff8/a1ab1fc1-7bbd-4a97-bab8-351a9b1dcc1c.png)](https://slid.cc/vdocs/113ad430f76e45319e6e6718db091ff8?v=83ea4d1b0e55461b870fa6ba948eba29&start=4686.316757143051)


집합 자료형과 관련된 추가적인 함수들도 있다. 새로운 원소 추가 add, 여러 개 추가 update, 특정 값 삭제 remove 등이 있다. 특히 이런 **집합 자료형의 경우 특정한 원소가 존재하는지 조회하거나, 추가 , 삭제 시 상수시간**이 걸린다는 점 기억하자!

[![이것이 코딩테스트다 (6) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/113ad430f76e45319e6e6718db091ff8/9ac1aae6-2871-402e-b12f-89cd162a9db2.png)](https://slid.cc/vdocs/113ad430f76e45319e6e6718db091ff8?v=83ea4d1b0e55461b870fa6ba948eba29&start=4727.584390141144)


기본적으로 리스트나 튜플은 순서가 존재하기 때문에 원소 접근 시 인덱싱을 사용할 수 있는데, **사전 자료형과 집합 자료형은 순서가 없기 때문에** ~~인덱싱을 사용할 수 없다.~~ 

**사전 자료형에 대해서는 키, 집합 자료형에 대해서는 원소를 이용해서 상수 시간**으로 값 조회 가능하다. 이때, 키나 원소의 값으로는 변경 불가능한 문자열이나 튜플과 같은 객체가 사용되야 한다는 점 기억해야한다!



