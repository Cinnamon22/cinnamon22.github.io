---
layout: post
title:  "백준 새싹문제"
date:   2022-09-15 22:53:00 +0900
categories: TIL
---
# 너무 피곤한 하루
아직 개강한 지 얼마 되지도 않았는데 너무 피곤해서 종강이 생각나는 하루였다. 요즘 아침형 인간이 되기 위해 기상시간을 당기고 운동을 시작한 것도 그 이유 중 하나 인 것 같다. 다음달부터 아침 수영을 배워보려고 계획 중인데 체력이슈가 심각해서 할 수 있을 지 고민 중이다. 어찌저찌 수업을 듣고 웨이트도 갔다가 스터디까지 마치고 나니 그대로 침대에서 기절해 있었다. 나는 정말 가만히 누워서 숨만 쉬고 있을 때가 가장 행복한데 굳이 이 험난한 세상을 열심히 살아야 되나 하는 쓸데없는 생각을 하다가 오늘 틈날때 마다 풀었던 백준 문제를 정리하려고 몸을 일으켰다.  
  


***

# 백준 새싹 문제
오늘 __solved.ac__ 에 들어가서 풀 만한 문제를 찾다가 새싹 문제라는 응애난이도 문제가 덜 풀려있는 것을 발견하고 모조리 정리했다. 최대한 지금 배우고 있는 언어인 _python_ 과 _C++_ 를 활용해 풀어보려고 노력했고 다행히 새싹 난이도여서 별 생각없이 언어에 익숙해 지는데 좋았다. 그 중 기억나는 두가지 문제만 정리해보도록 하겠다.  


## 대소문자 바꾸기
영어 소문자와 대문자로 이루어진 단어를 입력받은 뒤, 대문자는 소문자로, 소문자는 대문자로 바꾸어 출력하는 프로그램을 작성하시오.  

``` python
Q=input()
L=Q.lower()
C=Q.upper()
L=list(L)
Q=list(Q)
C=list(C)
A=[]
for x in range(len(Q)):
  if Q[x]==C[x]:
    A.append(L[x])
  else:
    A.append(C[x])
result=''.join(A)
print(result)
```

## 수 정렬하기 2
N개의 수가 주어졌을 때, 이를 오름차순으로 정렬하는 프로그램을 작성하시오.  

``` python
import sys
input=sys.stdin.readline

Arr=[]
N=int(input())
for x in range(N):
  Arr.append(int(input()))

Arr.sort()
for i in range(N):
  print(Arr[i])
```

***
오늘 문제를 풀며 느낀 점 중 하나는 python이 코딩테스트 문제를 풀기에 가장 편리한 언어라는 것이었다. C언어만으로 문제를 풀 때는 복잡하게 생각해야 한 것들이 단순한 코드 한 줄로 풀리는 것을 보며 python을 찬양하게 되었다. 물론 C++역시 행렬같은 문제를 풀 때 편리한 부분이 있는 것 같아 문제마다 적합한 언어를 찾는 것이 중요한 것 같다.  
  
오늘도 TIL을 쓰기 귀찮아 단돈 500원의 행복세를 내고 행복해지려 하였지만 최근 열심히 살겠다는 나의 다짐이 부끄러워져 TIL을 쓰고 있다. 요즘 또다시 인생 노잼시기가 도래한 것 같다. 모든 일에 별로 의욕도 없고 사람없는 무인도에서 열흘만 아무 생각없이 있고 싶다는 생각을 한다. 그래도 벌써 금요일인 만큼 주말에는 생각나는 아무 곳이나 여행을 가서 Refresh하려고 계획을 세웠다. 앞으로 좋은 일만 있는 하루가 되었으면 좋겠다.