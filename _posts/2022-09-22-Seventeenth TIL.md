---
layout: post
title:  "목요일 싫어~~"
date:   2022-09-22 22:46:00 +0900
categories: TIL
---
# 목요일 싫어~~
목요일은 수업 3개와 포리프 스터디가 있는 날이여서 아침부터 8시 반까지 밖에 있어야 한다. 목요일은 이것을 핑계로 저녁에 운동도 쉴 수 있는 건 좋은 것 같다. 요즘은 밖에서 숨만 쉬어도 에너지가 빠져서 들어와서 쉬고 싶은데 또다시 TIL을 적어야하는 내 신세를 생각하니 눈물이 차오르지는 않았다. 500원의 행복세를 내고 행복을 되찾을까 싶은 마음도 있었지만 TIL은 써야겠죠??  

***

오늘은 백준 1문제와 C++ 클래스를 살짝 공부했는데 여러언어를 동시에 공부하다보니 간단한 부분도 헷갈릴 때가 많은 것 같다. 예를 들어 C++에서 int main(){}을 안 적고 컴파일이 안 된다고 멍청한 소리를 하는 것처럼 python과 C++를 동시에 배우는 것은 좋지 않은 것 같다. 하지만 공창컴과 C++를 동시에 2학기에 배우고 시험쳐야 되는 상황이여서 덜 멀청하게 하려고 노력하는 방법밖에 없을 것 같다.

# 괄호
괄호 문자열(Parenthesis String, PS)은 두 개의 괄호 기호인 ‘(’ 와 ‘)’ 만으로 구성되어 있는 문자열이다. 그 중에서 괄호의 모양이 바르게 구성된 문자열을 올바른 괄호 문자열(Valid PS, VPS)이라고 부른다. 한 쌍의 괄호 기호로 된 “( )” 문자열은 기본 VPS 이라고 부른다. 만일 x 가 VPS 라면 이것을 하나의 괄호에 넣은 새로운 문자열 “(x)”도 VPS 가 된다. 그리고 두 VPS x 와 y를 접합(concatenation)시킨 새로운 문자열 xy도 VPS 가 된다. 예를 들어 “(())()”와 “((()))” 는 VPS 이지만 “(()(”, “(())()))” , 그리고 “(()” 는 모두 VPS 가 아닌 문자열이다. 

여러분은 입력으로 주어진 괄호 문자열이 VPS 인지 아닌지를 판단해서 그 결과를 YES 와 NO 로 나타내어야 한다. 

```python
T=int(input())
for x in range(T):
    count=0
    PS=input()
    for x in PS:
        if x=='(':
            count+=1
        else:
            count-=1
        if count<0:
            break
    if count!=0:
        print("NO")
    else:
        print("YES")
```

Just Easy~~ 포리프 스터디 때 딴 짓 하면서 풀었다. 준호씨는 못 볼테니 이렇게 고해성사 합니다. 준호야 미안해ㅠㅠ 다음부턴 제대로 들을께!!  


C++는 클래스 만드는 것을 다 잊어버려서 복습하는 중인데 위에서 언급한 것 같이 파이썬만 자주 쓰다보니 간단한 부분도 헷갈리는 부분이 많다. 자주 공부하도록 할께요.  
지금 배고파서 정신이 없는데 버거킹이 배달오기 전에 빠르게 TIL을 마무리하고 싶어서 이게 맞나 싶은 TIL을 쓰고 있는 중인데 내일은 수업도 3시에 끝나니까 공부 많이해서 좋은 TIL을 적겠습니다.  

## 금요일은 좋아~~!!^^