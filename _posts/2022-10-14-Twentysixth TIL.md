---
layout: post
title:  "공창컴 HW7"
date:   2022-10-14 23:41:00 +0900
categories: TIL
---

# 노트북 이슈
오늘은 오후에 데이터구조와 데이터베이스시스템 공부를 해보겠다고 생각했지만 예상치 못한 노트북 이슈가 생겼다. 데베시 강의를 듣던 중 갑자기 노트북 터치패트가 고장나서 노트북을 못쓰는 상황이 되었다. 임시방편으로 무선 마우스를 연결해서 사용했지만 빨리 고쳐야 되기에 공창컴 수업이 끝난 이후 서비스센터로의 여정을 떠났다.  
우선 가장 가까운 서비스센터가 용두역 근처에 있었는데 청계천을 따라 20분 정도 밖에 안걸려서 지하철 대신 따릉이를 타고 가기로 결심했다. 1년 정도만에 타는 자전거가 익숙하지 않아서 도착할 수 있을지 걱정했었는데 생각보다 자전거도로가 잘 되어 있어서 타고 가기에 좋았다. 하지만 오르막길이 있어서 돌아올 때는 반드시 지하철을 타겠다고 다짐하며 용두역에 도착했다.  
그리고 문앞에 붙어있는 휴무라는 안내를 보고 멘탈이 와장창 나가버렸다. 분명 네이버에는 영업중이라고 적혀있었는데... 미리 전화를 해야했다는 후회를 하며 다른 서비스센터를 찾아보니 다 애매한 거리에 있어서 그나마 가까운 군자역으로 지하철을 타고 향했다. 한양대역에서 바로 갔으면 훨씬 빨랐을텐데 환승에 환승을 거쳐서 서비스센터에 도착했다.  
괜히 쓸데없이 돈이 깨질 것을 걱정하고 있었는데 생각보다 훨씬 간단하게 수리가 끝났다. 그리고 놀랍게도 무료로 수리를 해주셔서 다행이었다. 그리고 서비스센터에서 노트북 파우치를 도난당했는데 한국에서 이런 일이 일어난다고?!라는 생각이 들었지만 어차피 낡은 파우치여서 기분 좋게 돌아왔다.

# 공창컴 HW7 과제
요즘따라 수업에 과제가 자주 나오는데 귀찮은 과제가 종종 등장하곤 한다. 이번 공창컴 과제 역시 귀찮은 부분이 많았는데 굳이 while 반복문 만을 사용해야 된다는 제약조건이 있어서 까다로웠다.  
그래도 한국어로 수업해줘서 감사한 공창컴 수업이라 나름 재미있게 과제를 했다.  
## 1번  
```python
print("(1)")
i=0
j=1
while i<7:
  while j<7-i:
    print(" ",end='')
    j+=1
  while 7-i<=j<=7+i:
    print("*",end='')
    j+=1
  while j<=13:
    print(" ",end='')
    j+=1
  print("")
  i+=1
  j=1
print("(2)")
i=0
j=1
while i<5:
  while j<i+1:
    print(" ",end='')
    j+=1
  while i+1<=j<=9-i:
    print("*",end='')
    j+=1
  while j<=9:
    print(" ",end='')
    j+=1
  print('')
  i+=1
  j=1
while i<9:
  while j<9-i:
    print(" ",end='')
    j+=1
  while 9-i<=j<=1+i:
print("*" end='')
```
## 2번
```python
i=1
j=1
while(j<=9):
  while (i<=3):
    print(i,'*',j,'=',i*j,end='\t')
    i+=1
  i=1
  j+=1
  print("")
  ```
## 3번
```python
import random
N=random.randint(1,100)

i=2
prime_list=[]
while i<=N:
  j=2
  check=1
  while j<i:
    if i%j==0:
      check=0
      break
    j+=1
  if check==1:
    prime_list.append(i)
  i+=1
print("발생된 난수:",N)
print("1에서 %d까지의 수 중에서 소수:"%N,end=' ')
k=0

while k<len(prime_list):
  print(prime_list[k],end=' ')
  k+=1
print("\n총 %d 개의 소수가 있습니다"%len(prime_list))
```
## 6번
```python
print("당신은 별다방에 왔습니다.\n")
print("---별다방 메뉴---")
print("[1] 아메리카노: 5500원")
print("[2] 카페라떼: 6000원")
print("[3] 카푸치노: 6500원")
print("[0] 종료\n")
next='y'
while(next=='y'):
  sum=0
  print("음료를 주문하세요.")
  name=input("당신의 이름: ")
  while(True):
    menu=int(input("메뉴 선택: "))
    if menu==0:
      break
    quan=int(input("수량 선택: "))
    if menu==1:
      cost=5500
    elif menu==2:
      cost=6000
    elif menu==3:
      cost=6500
    sum+=cost*quan
  print(name,"님의 총 요금은 %d 원 입니다"%sum)
  next=input("다음 손님 있습니까(y/n)? ")
```
이번주 주말에는 일정이 있어서 시험공부를 별로 못할 것 같긴 한데 우선 데이터구조와 데베시 과제만이라도 해결하는 것이 목표이다. 최근 TIL 안쓰고 세금내는 일이 많아졌는데 좀 더 성실히 써보겠습니다.  
그리고 세금이 밀리다 보니 내가 세금을 냈었는지 헷갈리는 지경에 이르렀는데 국세청에서 세금고지서 같은 거 알려주면 좋겠다. 성실납부!!!