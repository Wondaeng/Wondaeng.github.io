---
layout: single
title: "[찐막 Python] (1) Statement"
author: "wondaeng"
date: "2024-06-26 12:30:00 +0900"
---

# Iterators
파이썬의 container object들은 대부분 for문을 통해 iterate 될 수 있습니다:

```
for element in [1, 2, 3]:
    print(element)
for element in (1, 2, 3):
    print(element)
for key in {'one':1, 'two':2}:
    print(key)
for char in "123":
    print(char)
for line in open("myfile.txt"):
    print(line, end='')
```
하지만, 정확히 어떤 원리로 가능한 것일까요?

파이썬 공식문서를 보면 for statement를 다음과 같이 정의합니다.

```
for_stmt ::=  "for" target_list "in" starred_list ":" suite
              ["else" ":" suite]
```
