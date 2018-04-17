# Python-
Python编程
# 写一个函数 input_number读取数据放入列表L中

L = []
def input_number():    
    while True:
        i = int(input("请输入数字（-1结束）:"))
        if i == -1:
            return L
        L.append(i)
input_number()
print("您刚才输入的整数值是:",L)


# 2
def isprime(x):
    for y in range(2,x):
        if x % y == 0:
            return False
    return True
n = int(input("请输入一个大于零的数："))
if isprime(n):
    print("%d是素数" % n)


# 3

def prime_m2n(s,e):
    L = []
    for x in range(s,e):
        for y in range(2,x):
            if x % y == 0:
                break
        else:   
            L.append(x)
    return L
L = prime_m2n(10,20)
print(L)


# 4
def primes(n):
    L = []
    for x in range(2, n):
        for y in range(2, x):
            if x % y == 0:
                break
        else:    
            L.append(x)
    return L
L = primes(20)
