---
title: "이것이 코딩테스트다 (1)"
excerpt: "이것이 코딩테스트다 (1)"
toc: true
toc_sticky: true
categories:
  - 코딩테스트
tags:
  - Python
  - 나동빈
  - 코테
  - 코딩테스트
last_modified_at : 2021-04-27T17:50:00+05:00
---

https://www.youtube.com/watch?v=m-9pAwq1o3w&list=PLRx0vPvlEmdAghTr5mXQxGpHjWqSz0dgC

**이것이 코딩테스트다 - 나동빈**

강의를 듣고 나서 정리 겸 나중에 복습하기 위해 포스팅합니다!!

1. 코딩 테스트 출제 경향 분석 및 파이썬 문법 부수기

---

[![이것이 코딩테스트다 (2) - 알고리즘 성능 평가 image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/3c976c17fcee4b0cb055cea71de169d4/da09270c-2c09-444f-9990-bc1dbb41d6f3.png)](https://slid.cc/vdocs/960780469a8446969c2e28164c43f6cc?v=3681bf126a39475b9871422e8573cdca&start=1097.6217079122619)


기능이 동일하다면, 시간 혹은 공간 복잡도가 낮을수록 더 좋은 알고리즘이라고 알 수 있다.

[![이것이 코딩테스트다 (2) - 알고리즘 성능 평가 image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/3c976c17fcee4b0cb055cea71de169d4/c7141ccb-2575-4728-b19f-f9a183349e46.png)](https://slid.cc/vdocs/960780469a8446969c2e28164c43f6cc?v=3681bf126a39475b9871422e8573cdca&start=1109.8965980801086)


구체적으로 보자면 <span style="color:blue">Big-O 표기법</span>이 효과적으로 사용될 수 있다. 가장 빠르게 증가하는 항 만을 고려하는 표기법이라고 할 수 있다. 함수의 상한만을 나타내게 된다는 점이 특징이다. 추가적으로 계수는 무시하는데, 3N^3 이라면 N^3이라고 본다. 왜 이렇게 하느냐? N이 굉장히 큰 수라면? N^3을 제외한 나머지 수는 상대적으로 미미해 보일 것이다. 따라서 함수의 성능을 가늠해볼 수 있기 때문에 Big-O 표기법을 주로 사용한다.

[![이것이 코딩테스트다 (2) - 알고리즘 성능 평가 image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/3c976c17fcee4b0cb055cea71de169d4/ba82ed84-fa96-4002-913d-e66e921039f9.png)](https://slid.cc/vdocs/960780469a8446969c2e28164c43f6cc?v=3681bf126a39475b9871422e8573cdca&start=1223.5783169580384)


성능 상으로 좋은 것, 나쁜 것 표현해본 것이다. 여기서 나오는 명칭들은 기억해놓으면 도움이 될 것이다.

[![이것이 코딩테스트다 (2) - 알고리즘 성능 평가 image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/3c976c17fcee4b0cb055cea71de169d4/71dedb3b-daa9-4ff7-8b77-d5ff5f915ac1.png)](https://slid.cc/vdocs/960780469a8446969c2e28164c43f6cc?v=3681bf126a39475b9871422e8573cdca&start=1268.969193917984)


간단하게 시간복잡도를 계산해보는 예시를 보자. 간단하게 n개의 데이터가 존재할 때, 데이터를 모두 더한 값을 구하는 프로그램의 예제이다. 위 코드 상으로는 수행 시간은 데이터 개수 N에 비례할 것임을 예측할 수 있다. 따라서 시간 복잡도는 O(N)이다. 만약 N이 100만, 1억 이렇게 커진다면? 선형적으로 수행시간이 늘어나게 될 것이다. 또한 for문이 시간복잡도를 차지할 것임을 유추할 수 있다.

[![이것이 코딩테스트다 (2) - 알고리즘 성능 평가 image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/3c976c17fcee4b0cb055cea71de169d4/be35a6d6-e38f-4b3a-9ab8-4ba1b57e39b1.png)](https://slid.cc/vdocs/960780469a8446969c2e28164c43f6cc?v=3681bf126a39475b9871422e8573cdca&start=1386.7658670896453)


2중 반복문이라는 점에서 i \* j가 구해지는 횟수는 5 \* 5 = 25회이다. 따라서 시간복잡도는 O(N^2)이다. 여기서 알아두면 좋은 점은, 모든 2중 반복문의 시간 복잡도가 O(N^2)인 것은 아니다. 만약 안에 함수도 들어가 있다면, 함수의 시간 복잡도도 고려해줘야한다. 따라서 시간복잡도를 다시 체크해보는 것이 좋다.

[![이것이 코딩테스트다 (2) - 알고리즘 성능 평가 image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/3c976c17fcee4b0cb055cea71de169d4/2d5a292d-64c8-4b7f-8f24-558438d8f129.png)](https://slid.cc/vdocs/960780469a8446969c2e28164c43f6cc?v=3681bf126a39475b9871422e8573cdca&start=1489.0942199027252)


수행시간을 예측해가면서 알고리즘을 설계하는 것이 중요하다.

[![이것이 코딩테스트다 (2) - 알고리즘 성능 평가 image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/3c976c17fcee4b0cb055cea71de169d4/bb2ac577-192d-4cba-afd0-215e9f15cfec.png)](https://slid.cc/vdocs/960780469a8446969c2e28164c43f6cc?v=3681bf126a39475b9871422e8573cdca&start=1636.4452570877381)


요구사항에 따라 문제를 푸는 것이 중요하다. 데이터의 조건을 확인해야한다. 알고리즘 시간복잡도의 허용 기준? 을 가늠해볼 수 있기 때문이다.

[![이것이 코딩테스트다 (2) - 알고리즘 성능 평가 image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/3c976c17fcee4b0cb055cea71de169d4/a71507f3-ad2c-42cf-b739-055732ded6c5.png)](https://slid.cc/vdocs/960780469a8446969c2e28164c43f6cc?v=3681bf126a39475b9871422e8573cdca&start=1745.4178689923706)


먼저 지문을 꼼꼼히 읽고 컴퓨터적 사고로 문제를 잘게 분해해봐야한다. 그래서 문제를 최대한 간결하게 생각해보는 것이다. 여기서 기본적인 수학적 개념들이 활용될 수 있을 것이다.

[![이것이 코딩테스트다 (2) - 알고리즘 성능 평가 image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/3c976c17fcee4b0cb055cea71de169d4/864ac1e0-b07d-4eba-af6a-faa6ef31cd63.png)](https://slid.cc/vdocs/960780469a8446969c2e28164c43f6cc?v=3681bf126a39475b9871422e8573cdca&start=1846.7204919866485)


파이썬에서는 위와 같은 방식으로 시간을 계산해볼 수 있다.
