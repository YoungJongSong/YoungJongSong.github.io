---
title: "Song form"
categories :
    - "Music AI"
tags:
  - deep learning
  - Music Structure Segmentation
comments: true

---

먼저 모델이 song form을 구분할 수 있게 만들고 싶다.
그 이유는 음악 공부를 할때, 제일 먼저 배우는 것이 song form을 구분 하는 일이였던 것 같다.

song form을 잘 구분해 낸다면 가사 생성 모델이나 노래 생성 모델을 만들때에 도움이 될 것 같다.
요즘에는 작곡과 편곡을 나누는 개념이 모호해져서, 나누어서 생각하기에는 조금 애매하지만
작곡을 멜로디를 만드는 과정, 편곡은 사운드를 만드는 과정이라고 정의해보면
두가지 과정 모두 song form을 아는게 중요하다.

작곡에서 예를 들자면 모델이 song form을 잘 안다면 멜로디 생성 모델이 verse part에서는 전반적으로 잔잔한 멜로디를,  
음악에 main이 되는 chorus part는 대중성 있는 멜로디를 생성할 것 이다.

편곡에서도 마찬가지로 song form을 잘 안다면 같은 악기 구성이라도 , verse part에서는 잔잔한 사운드를,
pre-chorus part에서는 chorus part의 극대화를 위해 긴장감을 고조시키는 사운드를,
chorus part에서는 듣기 좋고 힘있는(다른 part보다 소스의 구성이 많아지는), 강렬한 사운드를 생성할 것 이다.

구글에서 좀 찾아보니 Music structure segment라는 분야로 연구가 진행되고있는 것 같다.
