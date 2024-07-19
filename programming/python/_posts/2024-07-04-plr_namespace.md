---
layout: single
title: "[Python] 공식문서 톺아보기 - (1) Expression VS Statement"
author: "wondaeng"
date: "2024-06-26 12:30:00 +0900"
---

# 여는 글

Python을 사용하다보면 수많은 변수를 만들게 됩니다. 그도 그럴것이, 애초에 프로그래밍 언어란 수많은 데이터를 다루기 위해 존재하는 거니까요. 

파이썬을 처음 배울 때, `a = 10` 이렇게 코드를 쓰면 a라는 변수에 10이라는 정수 값이 할당된다라고 배웠습니다. 당시에는 별다른 의문점 없이 넘어갔으나, 파이썬과 친해진 지 좀 된 지금은 조금 어색해 보이네요.

대부분의 수업과 온라인 자료에서는 이 등호 `=`를 `assignment operator`라고 부릅니다. 어떤 값을 변수에 할당하는 "일"을 하죠. 그런데... operator는 expression에 쓰는 것 아니었나요? 이 `a = 10`가 expression 이라면 자고로 하나의 값으로 eval이 되어야 하는건데 말이죠 -_-. 앞서말한 어떤 "일을 한다"라는 건 오히려 statement의 개념에 해당합니다. 헷갈리기 시작합니다.

이 무너진(ㅠㅠ) 저의 개념을 바로잡기 위해서 파이썬 공식문서를 다시 뒤져봤습니다.

이번 포스팅은 파이썬 공식문서:
[PEP 572 - Assignment Expression](https://peps.python.org/pep-0572/)
을 참고하였습니다.

# Rationale


