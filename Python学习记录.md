## 1. Python学习记录
### 1.1. Python流程控制
#### 1.1.1. if 语句
```
x = int(input('Please enter an integer:'))
if x < 0:
    x = 0
    print('Negattive changed to zero.')
elif x == 0:
    print('Zero.')
elif x == 1:
    print('Single.')
else:
    print('More.')
```
#### 1.1.2. for 语句
```
words = ['Congratulations', 'to', 'you']
for w in words:
    print(w, len(w))

for i in words[:]:
    if len(i) > 6:
        words.insert(0, i)
print(words)
```
#### 1.1.3. range() 函数
```
# for i in range(5):  # 表示0到4
# for i in range(5, 10):
# for i in range(0, 10, 3):
for i in range(-10, -100, -30):
    print(i)
```
```
a = ['Congratulations', 'to', 'you']
for i in range(len(a)):
    print(i, a[i])
```
###  break 和 continue 语句, 以及循环中的 else 子句
```
for n in range(2, 10):
    for x in range(2, n):
        if n % x == 0:
            print(n, 'equals', x, '*', n // x)
            break
    else:
        print(n, 'is a prime number')
```
