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

# 문자열, 튜플 자료형

[![이것이 코딩테스트다 (5) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/3fdcd30b37534da89c2b3b59428b2597/e1afe263-3674-4107-88d2-e0a9e22037e9.png)](https://slid.cc/vdocs/3fdcd30b37534da89c2b3b59428b2597?v=83ea4d1b0e55461b870fa6ba948eba29&start=3844.584874026703)


다른 언어들은 " 으로 문자열, '로 문자 하나를 쓰는데, 파이썬은 구분을 안둔다.

[![이것이 코딩테스트다 (5) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/3fdcd30b37534da89c2b3b59428b2597/cb26c56d-eec3-4540-b35b-c510161d21eb.png)](https://slid.cc/vdocs/3fdcd30b37534da89c2b3b59428b2597?v=83ea4d1b0e55461b870fa6ba948eba29&start=3904.0616249523164)

[![이것이 코딩테스트다 (5) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/3fdcd30b37534da89c2b3b59428b2597/a15bf506-4453-4022-8a9b-faf32e5748e2.png)](https://slid.cc/vdocs/3fdcd30b37534da89c2b3b59428b2597?v=83ea4d1b0e55461b870fa6ba948eba29&start=3971.26802397139)


문자열에 대해서도 인덱싱과 슬라이싱을 이용할 수 있다! 다만 수정은 못한다는 점 유의해야 한다.

[![이것이 코딩테스트다 (5) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/3fdcd30b37534da89c2b3b59428b2597/aa737273-5459-4e16-9892-9d6d31aee8be.png)](https://slid.cc/vdocs/3fdcd30b37534da89c2b3b59428b2597?v=83ea4d1b0e55461b870fa6ba948eba29&start=4000.589424070572)


문자열끼리 붙일 때는 "+", 문자열 반복은 "\*", 문자열의 슬라이싱 또한 \[:\] 가능하다.

[![이것이 코딩테스트다 (5) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/3fdcd30b37534da89c2b3b59428b2597/585ad961-afa6-47ad-bdae-1547a2d8c218.png)](https://slid.cc/vdocs/3fdcd30b37534da89c2b3b59428b2597?v=83ea4d1b0e55461b870fa6ba948eba29&start=4083.8009879847414)


파이썬은 튜플이라는 특이한 자료형이 존재한다. 튜플은 한 번 선언된 값을 변경할 수 없다는 특징이 있다. 문자열과 마찬가지라고 생각하면 된다. 

리스트는 가능했지만, 튜플은 불가능하다. 또한 리스트는 대괄호(\[\]), 튜플은 소괄호(())를 이용한다. 

또한 튜플은 리스트에 비해 기능이 제한적이기 때문에 공간효율적이라는 특징이 있다. 일반적으로 리스트보다 더 적은 메모리를 사용한다는 말이다.

[![이것이 코딩테스트다 (5) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/3fdcd30b37534da89c2b3b59428b2597/e21b9954-1cc4-425e-ad09-ab9ce93875db.png)](https://slid.cc/vdocs/3fdcd30b37534da89c2b3b59428b2597?v=83ea4d1b0e55461b870fa6ba948eba29&start=4134.862809885559)

[![이것이 코딩테스트다 (5) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/3fdcd30b37534da89c2b3b59428b2597/d2a7639c-c7d5-4de1-98ad-6fc5f7f96d85.png)](https://slid.cc/vdocs/3fdcd30b37534da89c2b3b59428b2597?v=83ea4d1b0e55461b870fa6ba948eba29&start=4168.595905204086)


튜플은 변경불가능한 객체이므로 원소 할당 연산은 지원하지 않는다는 오류 메세지를 확인할 수 있다.

[![이것이 코딩테스트다 (5) image](https://slid-capture.s3.ap-northeast-2.amazonaws.com/public/capture_images/3fdcd30b37534da89c2b3b59428b2597/9f98ec27-2976-470a-9ea5-e8c29cdb4a98.png)](https://slid.cc/vdocs/3fdcd30b37534da89c2b3b59428b2597?v=83ea4d1b0e55461b870fa6ba948eba29&start=4181.106770049591)


어떤 경우에 튜플을 사용하면 좋을까? 일반적으로 파이썬 커뮤니티에서 말하는 튜플의 사용법이다. 리스트와 다르게 튜플은 일반적으로 서로 다른 성질의 데이터를 묶어서 관리해야할 때 사용한다. 

일반적으로 최단경로 알고리즘에서는 비용을 실수값으로 저장할 수 있고, 노드 번호는 정수형태로 처리한다고 하면 하나로 묶어서 사용할 때 튜플 자료형을 사용한다.

또한 학생 정보라면 학번, 이름 등을 하나로 묶어서 관리할 때 튜플 자료형이 사용된다는 점을 기억하면 좋겠다. 

또한 사전자료형, 집합자료형 등에서 데이터의 묶음, 나열을 사용할 때 튜플을 사용한다. 

리스트와 달리 변경이 불가능하므로 해싱 연산에서 키 값으로 사용 가능하다. 추가적으로 리스트보다 메모리를 더 효율적으로 사용해야할 때 튜플을 사용하면 좋다.

