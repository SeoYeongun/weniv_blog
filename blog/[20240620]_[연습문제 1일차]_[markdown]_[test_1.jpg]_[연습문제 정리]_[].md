# 03.10 연습문제

- - -

## 1번 문제

다음 변수들이 가리키고 있는 값에 화살표를 그려주세요. z의 값은 무엇인지도 유추해보세요.

```python
x = 100
y = 100
z = x
```

## 2번 문제

다음 파이썬 문법 중 맞은 것을 골라주세요.(3개)

```python
#1번
print = 100
 
#2번
10 = a
 
#3번
k = 100
 
#4번
100k = 10000
 
#5번
a123 = 'abc'
 
#6번
_ = 10
```

## 3번 문제

문자를 사용자에게 입력받고, 그 문자를 2번 출력하는 프로그램을 만들어주세요. 예를 들어 ‘abc’를 입력받는다면 ‘abcabc’를 출력해야 합니다.

## 4번 문제

아래 변수에서 중복을 제거한 유일한 숫자를 알아내는 코드를 작성해주세요. 형변환을 통해 풀어주세요.

```python
n = 1234567890123123123
```

## 5번 문제

문자열 s에 마지막에 있는 문자열을 2번 더 붙이는 코드를 작성해주세요.

```python
s = 'jun'
# 출력값: 'junnn'
```

## 6번 문제

'abcde', 숫자, 대쉬(-), 언더스코어(_)를 모두 제거해주세요. 문자열에 translate를 사용해주세요.

```python
s = 'hello_world123'
# 출력값: 'hlloworl'
```

# 7번 문제

확장자를 출력해주는 코드를 작성해주세요. 확장자는 png, jpeg, mp4 등입니다.

```python
s = 'licat.jpeg'
# 출력값: 'jpeg'
 
s = 'li.cat.png'
# 출력값: 'png'
```

- - -

1.

```python
# 정답
# z ┐
# x -> 100
# y ┘
x = 100
y = 100
z = x
 
print(id(x), id(y), id(z))
```
```python
# 문제2
x = 258
y = 258
z = x
```
```python
# 정답
# z ┐
# x -> 258
# y -> 258
x = 258
y = 258
z = x
 
print(id(x), id(y), id(z))
```
2.
```python
# 정답: 3번, 5번, 6번
```
3.
```python
# 정답
user_input = input()
user_input * 2
```
4.
```python
# 정답
n = 1234567890123123123
len(set(str(n)))
```
5.
```python
# 정답
s = 'jun'
s = s + s[-1] * 2
print(s)
```
6.
```python
# 정답
s = 'hello_world123'
table = str.maketrans('', '', 'abcde0123456789-_')
s.translate(table)
```
7.
```python
s[::-1].split('.')[0][::-1] # 정답1
s.split('.')[-1] # 정답2
s[s.rindex('.')+1:] # 정답3
```
