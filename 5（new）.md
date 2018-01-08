

```python
#练习1 写函数，求n个随机整数均值的平方根，整数范围在m与k之间（n,m,k由用户输入）。
import random,math

def my_function():
    n=int(input('请输入你想输入的整数个数'))
    i=0
    sum=0
    while i<n:
        a=random.randint(m,k)
        sum+=a
        i+=1
    b=math.sqrt(sum/n)
    return b

m=int(input('请输入随机整数的下限'))
k=int(input('请输入随机整数的上限'))
my_function()
```

    请输入随机整数的下限3
    请输入随机整数的上限7
    请输入你想输入的整数个数23
    




    2.255428234668337




```python
#练习2：写函数，共n个随机整数，整数范围在m与k之间，（n,m,k由用户输入）。求1：西格玛log(随机整数)，2：西格玛1/log(随机整数)

import random,math
def FUNCTION_b():
    m=int(input('请输入随机范围的最小值'))
    k=int(input('请输入随机范围的最大值'))
    n=int(input('请输入你想去的随机数的个数'))
    
    i=0
    total=0
    while i<n:
        i+=1
        b=random.randint(m,k)
        c=math.log2(b)
        total=total+c
    
    return total

print(FUNCTION_b())
print(1/FUNCTION_b())
```

    请输入随机范围的最小值3
    请输入随机范围的最大值90
    请输入你想去的随机数的个数455
    2352.0202385490534
    请输入随机范围的最小值34
    请输入随机范围的最大值666
    请输入你想去的随机数的个数34
    0.003672490025521922
    


```python
#练习 3：写函数，求s=a+aa+aaa+aaaa+aa...a的值，其中a是[1,9]之间的随机整数。例如2+22+222+2222+22222(此时共有5个数相加)，几个数相加由键盘输入。

import math,random

def freak():
    n=int(input('请输入你想要数字的个数'))
    a=random.randint(1,10)
    print(a)
    i=0
    b=0
    sum=0
    while i<n:
        b=a*(10**i)+b
        sum+=b
        i+=1
    return sum

freak()
```

    请输入你想要数字的个数4
    7
    




    8638


