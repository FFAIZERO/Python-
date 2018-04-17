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
