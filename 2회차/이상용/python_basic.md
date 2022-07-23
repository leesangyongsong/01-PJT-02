# 📚 Jump to 'PYTHON'

## 📌 1. 파이썬 시작하기

    ```
    - '귀도 반 로섬'이 취미로 만든 프로그래밍 언어
      - 1991년 최초 발표
      - 2000년 python 2, 2008년 python 3 version-upgrade
    - 구글에서 만들어진 소프트웨어의 50% 이상이 파이썬
    - 드롭박스(Dropbox), 인스타그램(Instagram) 등
    - 이해하기 쉬워 공동 작업과 유지 보수가 편하다.
    ```
### 1-1. 파이썬의 특징

1) 파이썬은 인간다운 언어이다
    ```python
    if 4 in [1,2,3,4]: print("4가 있습니다") 
    => 만약 4가 [] 안에 있으면 ("4가 있습니다")를 출력해라
    ````
2) 파이썬은 문법이 쉬워 빠르게 배울 수 있다
    ```
    - 대학교 교양 강의로 파이썬 활용
    - 프로그래밍 유 경험자라면 1주일이면 충분
    ```
3) 파이썬은 무료지만 강력하다
    ```
    - 사용료 걱정없이 언제 어디서든 파이썬을 다운로드하여 사용
    - 파이썬과 C는 찰떡궁합(접착언어)
      - 파이썬은 쉬운데 느리고, C는 빠른데 복잡함
      - 상대적으로 쉽지만 느린 파이썬 + 빠른 C언어 조합 가능
    - 파이썬 라이브러리들 중에는 C로 만들어진 것도 많다.
      - NumPy: C라이브러리를 python에서 쓸 수 있도록 래핑
    ```
4) 파이썬은 간결하다.
    ```python
    # simple.py
    languages = ['python', 'perl', 'c', 'java']
    for lang in languages:
      if lang in ['python', 'perl']:
        print("%6s need interpreter" % lang)
      elif lang in ['c', 'java']:
        print("%6s need compiler" % lang)
      else:
        print("should not reach here")

    - 파이썬은 가장 좋은 방법 1가지만 이용하는 것을 선호
    - 실행이 되게 하려면 꼭 줄을 맞추어야 한다.(다른 언어에 비해 엄격한 면이 있음)
    ```
5) 파이썬은 개발 속도가 빠르다
    ```
    - "Life is too short, You neeed python."

### 1-2. 파이썬으로 무엇을 할 수 있을까?
```
- 파이썬으로 할 수 있는 일   
  - 시스템 유틸리티 제작 ex) 고클린 등의 시스템 청소 도구
  - GUI(graphical user interface) 프로그래밍
  : 사용자가 편리하게 사용할 수 있도록 기능을 그래픽으로 나타낸 것
  - C/C++와의 결합
  - 웹 프로그래밍 ex) django, flask
  - 수치 연산 프로그래밍 ex) SQL
  - 데이터베이스 프로그래밍
  - 데이터 분석, 사물 인터넷(IOT) 
  IOT: 각종 사물에 센서와 통신 기능을 내장하여 인터넷에 연결하는 기술

- 파이썬으로 할 수 없는 일
  - 시스템과 밀접한 프로그래밍 영역 ex) OS - Window, Linux
  - 모바일 프로그래밍 ex) App 제작
```

### 1-3. 파이썬 설치하기
```
- 파이썬 언어 패키지를 다운로드한다.
- 파이썬이 어느 곳에서든지 실행될 수 있도록 "Add Python 3.8 to PATH" 옵션을 선택한다.
```

## 📌 2. 자료구조
| 자료에 대한 타입 | 어떤 값을 담는 자료구조 |
| --- | ----|
| 숫자, 문자열, 불 | 변수, 리스트, 튜플, 딕셔너리, 집합 |

> 리스트 : 변수 여러 개를 묶는 역할

### 2-1. 숫자형
  ```python
- 정수형(int)
- 실수형(float)
- 컴퓨터식 지수 표현 방식
- 8진수
- 16진수
  ```

### 2-2. 문자형
  ```python
  str 로 표시되며, "" or '' 둘 다 표시 가능

  - Indexing
  - Slicing [이상:미만:간격] # 간격은 생략가능
  ```

문자열 함수
| 함수명 | 기능 |
| ---- | ----- |
| count | 문자열 개수 세기 |
| find | 문자열 위치 알려주기 |
| join | 문자열 삽입 |
| upper | 소문자 -> 대문자 변경 |
| lower | 대문자 -> 소문자 변경 |
| strip | 양쪽 공백 지우기
| replace | 문자열 바꾸기 |
| split | 문자열 나누기 |

### 2-3. 리스트 자료형

리스트 함수
| 리스트 함수명 | 기능 |
| --- | --- |
| append | 리스트 맨 뒤에 요소 추가 |
| sort | 리스트 정렬 : 문자는 ㄱㄴㄷ순, 숫자는 크기 순|
| reverse | 리스트 순서 뒤집기 |
| index | 위치 반환 |
| insert | 리스트 특정 위치에 요소 추가 |
| remove | 리스트 내 요소 제거 |
| pop | 리스트 내 마지막 요소 제거 |
| extend | 리스트 확장 |

### 2-4. 튜플형 자료형
```python
리스트와 유사하나 차이점이 있음.

- 리스트는 [대괄호], 튜플은 (소괄호) 사용
- 리스트는 내역 변경이 가능하나, 튜플은 불가능(단, 인덱싱 및 슬라이싱은 가능)
```

### 2-5. 딕셔너리 자료형📝 (중요!)
``` python
- 연관 배열(Associative array) 또는 해시(Hash)
- 단어 그대로 해석하면 사전이라는 뜻
- Key를 통해 Value를 얻는다

>>>  a = {
          'name': 'pey',
          'phone': '0119993323',
          'birth': '1118'
          }

◆ 딕셔너리 쌍 추가하기
>>> a = {1: 'a'}
>>> a[2] = 'b'
>>> a
{2: 'b', 1: 'a'}

◆ 딕셔너리 요소 삭제하기
>>> a = {1: 'a'}
>>> a['name'] = "익명"
>>> del a[1]
>>> a
{'name': '익명'}

◆ 딕셔너리에서 key 사용해 value 얻기
>>> grade = {'pey': 10, 'julliet': 99}
>>> grade['pey']
10
>>> grade['julliet']
99

◆ 딕셔너리 만들 때 주의할 사항
>>> a = {1: 'a', 1: 'b'}
>>> a
{1: 'b'} 
# 같은 키가 중복될 경우 마지막에 매칭된 key와 value값으로 인식된다. 
# 딕셔너리는 key값으로 인식하기 때문에 key값을 '반드시' 다르게 해야 한다. 
# (여러 key 값에 같은 value는 가능)

◆ Key 리스트 만들기(keys)
>>> a = {
        'name': 'pey',
        'phone': '0119993323',
        'birth': '1118'
        }
>>> a.keys()
dict_keys(['name', 'phone', 'birth'])

◆ Value 리스트 만들기(values)
dict_values(['pey', '0119993323', '1118'])

◆ Key, Value 쌍 얻기(튜플 형태)
dict_itmes([('name': 'pey'), ('phone': '0119993323'), ('birth': '1118')])

◆ Key, Value 쌍 모두 지우기(clear)
>>> a.clear()
>>> a
{} # 빈 딕셔너리가 됌

◆ 해당 Key가 딕셔너리 안에 있는지 조사하기(in)
>>> a = {
        'name': 'pey',
        'phone': '0119993323',
        'birth': '1118'
        }
>>> 'name' in a
True
>>> 'email' in a
False
```

### 2-6. 집합 자료형
```python
집합의 핵심: 
- 집합에 관련된 것들을 쉽게 처리하기 위해 만들어진 자료형(파이썬에만 有)
- 중복을 허용하지 않는다.
- 순서가 없다(unordered)

◆ 집합 자료형
>>> s1 = set([1, 2, 3])
>>> print(s1)
{1, 2, 3}
# list를 set으로 감싸면 집합으로 변환

>>> 1 = [1,2,2,3,3]
>>> newList = list(set(1))
>>> print(newList)
[1, 2, 3]
# set으로 중복값을 없앤 후 다시 리스트로 변환

>>> s1 = set('Hello')
>>> print(s1)
{'o', 'l', 'e', 'H'}

◆ 교집합
>>> s1 = set([1, 2, 3, 4, 5, 6])
>>> s2 = set([4, 5, 6, 7, 8, 9])
>>> print(s1 & s2) or print(s1.intersection(s2)) # 교집합 구하기
{4, 5, 6}

◆ 합집합
>>> s1 = set([1, 2, 3, 4, 5, 6])
>>> s2 = set([4, 5, 6, 7, 8, 9])
>>> print(s1 | s2) or print(s1.union(s2)) # 합집합 구하기
{1, 2, 3, 4, 5, 6, 7, 8, 9}

◆ 차집합
>>> s1 = set([1, 2, 3, 4, 5, 6])
>>> s2 = set([4, 5, 6, 7, 8, 9])
>>> print(s1 - s2) or print(s1.difference(s2)) # 차집합 구하기
{1, 2, 3}

◆ 값 추가하기
>>> s1 = set([1, 2, 3])
>>> s1.add(4) # 값 1개 추가하기 add
>>> print(s1)
{1, 2, 3, 4}

>>> s1 = set([1, 2, 3])
>>> s1.update([4, 5, 6]) # 값 여러 개 추가하기 update
>>> print(s1)
{1, 2, 3, 4, 5, 6}

◆ 값 제거하기
>>> s1 = set([1, 2, 3])
>>> s1.remove(2) # 값 제거하기 remove
>>> print(s1)
{1, 3}
```

### 2-7. 불리언 자료형(불)
| 구분 | 값 | 참 or 거짓 |
| --- | -- | ----- | 
| 문자열_str | "python" | 참 |
| 문자열_str | " " | 거짓 |
| 리스트_list | [1, 2, 3] | 참 |
| 리스트_list | [] | 거짓 |
| 튜플_tuple | () | 거짓 |
| 딕셔너라_dictionary | {} | 거짓 |
| 숫자열 | 1(그 외 1 이상의 수) | 참 |
| 숫자열 | 0 | 거짓 |
| 불 | None | 거짓

### 2-8. 변수
```python
변수: 자료형의 값을 저장하는 공간

파이썬에서 사용하는 변수는 객체를 가리키는 것
>>> a = 3

- 3이라는 값을 가지는 정수 자료형(객체)이 자동으로 메모리에 생성
- 변수 a는 객체가 저장된 메모리의 위치를 가리키는 레퍼런스(Reference)
- a라는 변수는 3이라는 정수형 객체를 가리키고 있다

# 변수의 활용 : case1
>>> a = [1, 2, 3]
>>> b = a
>>> a[1] = 4 # b가 a의 주소를 가져오는 것이기 때문에 a의 리스트 내역이 바뀌면 b도 같이 변경된다!
>>> print(a)
>>> print(b)
[1, 4, 3] # a의 리스트
[1, 4, 3] # b의 리스트

# 변수의 활용 : case2
>>> a = [1, 2, 3]
>>> b = a[:] # a를 슬라이싱한 값을 b에 넣어 새로운 값을 얻음
>>> a[1] = 4 
>>> print(a)
>>> print(b)
[1, 4, 3] # a의 리스트
[1, 2, 3] # b의 리스트
```

## 📌 3. 제어문
| 구분 | 내역 |
| ---- | ---- |
| 조건문 | ~하면 ~해라 |
| 반복문 | ~하는 동안 ~ 해라 |


### 3-1. 조건문
```python
돈이 있으면 택시를 타고, 돈이 없으면 걸어간다!
>>> money = True
>>> if money:
      print("택시를 타고 간다")
    else:
      print("걸어간다!")
```

### 3-2. 반복문
| 구분 | 내역 |
| ---- | ---- |
| for문 | 순회할 때 (문자열/리스트 등) + 횟수를 알 때(range) |
| while문 | 조건에 도달할 때까지(while True + break) |

```python
나무를 10번 찍는다
>>> treeHit = 0
>>> while treeHit <=1:
      treeHit += 1
      print("나무를 &d번 찍었습니다" % count)
      if treeHit == 10:
      print("나무가 쓰러졌습니다.")
```

### 3-3. 이중반복문
```python
구구단 만들어보기
>>> for i in range(2, 10):
      print(f"{i}단")
      for j in range(1, 10):
        print(f"{i} '*' {j} '=' '{i * j}' ")

구구단 리스트에 넣기
>>> result = []
    for x in range(2,10):
      for y in range(1, 10):
        result.append(x * y)

# 한줄로 표현하면?
>>> result = [x * y for x in ragnge(2, 10) for y in range(1, 10)]
```

## 📌 4. 함수
### 4-1. 파이썬 함수의 구조
```python

def 함수명(매개변수):
  <수항핼 문장1>
  <수항핼 문장2>
  ...
  return 리턴 값

ex)
>>> def sum(a, b):
      result = a + b
      retrun result
    print(sum(1,2))
3

# 함수의 결과값은 항상 하나!
>>> def sum_and_mul(a,b):
      return a+b, a*b # 리턴 값이 두개일 때는
    print(sum_and_mul(1,2))
(3, 2) #tuple 형태로 1개의 결과값 출력

# 매개 변수에 초기값 미리 설정하기
>>> def say_myself(name, old, man=True): # 초기값을 미리 설장한다면?
      print("나의 이름은 %s 입니다." % name)
      print("나이는 %d 입니다." % old)
      if man:
        print("남자입니다.")
      else:
        print("여자입니다.")
    say_myself("라이유튜브", 20) # 함수 사용시 별도로 인자가 없어도 실행! 

# 함수 안에서 선언된 변수의 효력 범위
>>> a = 1
    def vartest(a):
      a = a + 1
    vartest(a)
    print(a)
1 # return 값이 없으면 함수는 외부 변수에 영향을 줄 수 없음

# Lambda 함수: 함수를 간단하게 표현하는 방법
>>> add = lambda a, b : a+b
    result = add(3,4)
    print(3, 4)
7

# 아래와 완전히 동일
>>> def add(a, b):
      return a + b
```

### 4-2. 사용자 입력과 출력
```python
# input의 사용, input: 입력을 받는 내장함수
>>> a = input()
Life is too short, you need python
>>> print(a)
'Life is too short, you need python'

# print문
>>> print("life" "is" "too short")
lifeistoo short
>>> print("life"+"is"+"too short")
lifeistoo short
>>> print("life", "is", "too short")
life is too short
>>> for i in range(10):
      print(i, end=' ')
0 1 2 3 4 5 6 7 8 9
```

### 4-3. 파일 읽고 쓰기
| 파일열기모드 | 설명 |
| --- | --- |
| r | 읽기모드 - 파일을 읽기만 할 때 사용 |
| w | 쓰기모드 - 파일에 내용을 쓸 때 사용 |
| a | 추가모드 - 파일의 마지막에 새로운 내용을 추가 시킬 때 사용 |

```python
# 파일 생성하기
f = open("새파일.txt", "w") 
# 상대경로: 현재 실행하는 파일을 기준으로 상대적인 경로를 써주는 것
f.close()

# 파일을 쓰기 모드로 열어 출력값 적기
f = open("C:/Python/새파일.txt", 'w', encoding="UTF-8") 
# 절대경로: 처음부분(C:/)부터 주소를 써주는 것
for i in range(1, 11):
  data = "%d번째 줄입니다.\n" % i
  f.write(data)
f.close()

# 파일 읽기
readline(): 한줄 읽는 것
readlines(): 리스트 형태로 가져와서 출력
read(): 통째로 가져오는 것

# 파일 추가/수정
f.write()

# close를  안하는 방법
with open("foo.txt", "w") as f:
  f.write("Life is too short, you need python")
```