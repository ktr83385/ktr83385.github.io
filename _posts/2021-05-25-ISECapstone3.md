---
title: "산업시스템공학종합설계 중간발표 (1)"
excerpt: "산업시스템공학종합설계 세 번째 게시글"
toc: true
toc_sticky: true
categories:
  - 산업시스템공학종합설계
tags:
  - 산업시스템공학종합설계
  - 졸업프로젝트
  - 산업공학
  - 중간발표
  - 1등!!!
last_modified_at : 2021-05-25T11:50:00+05:00
---

> 5월 13일 **산업시스템공학종합설계 중간 발표 자료를 제출했다.** 4월 12일 두 번째 포스팅 이후 중간 발표 이야기로 5월 25일인 오늘 세 번째 포스팅을 하려 한다. 저번에 최종 제안서에서 확정 지은 우리의 종합설계 주제는 **"딥러닝을 활용한 어린이 낙상 사고 유형 분석 시스템 개발"이다.** 본론부터 말하자면, 5월 22일에 나온 중간 결과에서 총 13팀 중 **우리 팀이 1등했다!!!!**

※ 이전 포스팅

[산업시스템공학종합설계 최종 제안서](https://ktr83385.github.io/%EC%82%B0%EC%97%85%EC%8B%9C%EC%8A%A4%ED%85%9C%EA%B3%B5%ED%95%99%EC%A2%85%ED%95%A9%EC%84%A4%EA%B3%84/ISECapstone2/)

이번 중간 발표를 준비하면서 가장 어려웠던 점은 **슬라이드 11P와 5분이라는 발표시간 동안에 우리의 프로젝트를 녹여야한다**는 점이었다. 말할 내용은 많은데... 진짜 핵심만 보여달라는 교수님들의 의중을 알 수 있었다. ~~덕분에 밤을 샜습니다~~

# 중간 발표 PPT

## 1P 주제

![image](https://user-images.githubusercontent.com/55723966/119430269-70f17000-bd4b-11eb-94a8-74e279027ca4.png)

프로젝트 주제는 **"딥러닝을 활용한 어린이 낙상 사고 유형 분석 시스템 개발"**이다. 우리는 객체 탐지 모델인 Yolov5와 행동 인식 모델 Slowfast를 결합하여 **낙상을 감지하고 더 나아가 낙상의 원인이 무엇인 지를 분석**하는 것을 방향으로 잡았다.

## 2P 목차

![image](https://user-images.githubusercontent.com/55723966/119430338-8e263e80-bd4b-11eb-87a8-7b5195321dc8.png)

목차는 감사하게도, 교수님이 주신 가이드라인을 토대로 만들었다. 

## 3P 연구 배경 및 문제 정의

![image](https://user-images.githubusercontent.com/55723966/119431418-82d41280-bd4d-11eb-8fc1-5316206b54fb.png)

### 문제 정의 도출 과정

우리가 만든 자료가 어떤 수준인 지 감이 안와서, 중간 자료를 제출하기 3일 전부터 초안을 만들어본 뒤, 학과의 여러 교수님들께 메일을 드려 피드백을 받았었다. 그 중, 문제 정의 도출 과정에서 **"낙상 사고 감지 및 원인 분석 시스템 부재"가 어떻게 결론인 지 이해가 안간다**는 말이 있었다. 

따라서 이에 대한 자료조사를 다시 한 뒤, 

* 어린이의 낙상 사고가 잦은 것
* 사고 유형 파악의 중요성 
* 현재 연구 동향을 살펴보면 낙상을 "감지"하는 것에 그치고 있다

위의 항목들을 묶어 **어린이 낙상 사고 유형 분석 시스템의 부재**를 문제로 도출해냈다. 연구배경 및 문제 정의 부분에서 좋은 점수를 받을 수 있었다.

## 4P 연구 목표

![image](https://user-images.githubusercontent.com/55723966/119431992-7ef4c000-bd4e-11eb-9e5c-3c3bb7f676a8.png)

목차 중에는 "연구 목표"와 "프로젝트 목표"가 있었다. 이 둘의 차이점을 곰곰히 생각해보고, 교수님이 주신 가이드라인을 재차 읽어본 결과 "연구 목표"는 좀 더 큰 범주의 목표, "프로젝트 목표"는 구체화 시킨 세부 목표를 포함해야 한다는 결론을 냈다. 우리의 연구는 크게 위와 같은 방식으로 진행될 것임을 정리했다.

## 5P 프로젝트 목표

![image](https://user-images.githubusercontent.com/55723966/119585774-592af200-be06-11eb-864a-409f1fc23a1f.png)

프로젝트 목표를 보면 놀이터 영상에서~, 감지를 통한~ 등의 문구가 추가되어 좀 더 구체적으로 적혀 있는 것을 볼 수 있다. 

### 프로젝트 범위를 위한 가정

우리는 **낙상 유형을 분석하는 시스템**을 만들건데, 그 중에서도 **놀이터에 특화되게** 만들고 싶다는 것이다. *왜 굳이 놀이터냐?* 이것은 가정 중 한가지다. 이 외에도 여러 가정들이 있다.

1. 놀이터에서 발생하는 것만 다룬다.
   - 프로젝트의 범위를 확실히 하기 위해서 놀이터를 선정했다.
2. "쓰러짐" 상태는 낙상으로 판단한다.
   - 낙상이 아님에도 놀이 차원에서 누워 있을 수도 있기 때문에 "5초 이상 쓰러져 있을 시"라는 조건을 달았다.
3. 5초 이상 쓰러져 있을 시 위험 상황이라 판단.

4. "쓰러짐 상태가 5초 이상 지속 시(위험 상황) 사고 유형을 분석

5. 낙상은 넘어짐(전방/후방) , 추락(머리/다리) 총 4가지로 분류한다. 
    * 이 4가지만 낙상으로 간주하는 이유는 역시 프로젝트 범위를 명확하게 하기 위해서다.

### 프로젝트 세부 목표

이러한 가정들 속에서 세부 목표는 3가지가 있다.

1. Yolov5 모델의 쓰러짐 감지 정확도 90% 이상

2. SlowFast 모델의 낙상 유형 분석 정확도 85% 이상

3. 모델의 정확도를 높이기 위한 낙상 관련 다양한 데이터를 수집

이처럼 프로젝트 범위와 목표를 구체적으로 나타낸 점이 중간 고사에서 좋은 점수를 받는데 일조했다고 생각한다.

--- 

> 연구 방법론부터는 다음 포스팅에..!!!