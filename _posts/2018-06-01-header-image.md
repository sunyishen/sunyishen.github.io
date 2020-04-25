---
title: python编程：从入门到实践 笔记
tags: python
article_header:
type: cover

---


## 第二章：变量和数据类型


变量名只能包含 **字母 数字 下划线**，开头不能是数字。

<!--more-->

### 字符串

```python
name = "hello world"
print(name.title())                #首字母大写
print(name.upper())                #全大写
print(name.lower())                #全小写

name_1 = "goodbye"
name_2 = name +" "+ name_1                #合并字符串

strip()                #去掉字符串两边的空白
rstrip()            #去掉右边
lstrip()            #去掉左边
```

### 数字

加（+）减（-）乘（*）除（/）乘方（**）运算

```python
age = 23
str(age)                #转换成字符串类型
```

## 第三章 列表简介

### 列表

用方括号 [ ] 来表示列表，并用逗号来分隔其中的元素，索引从0开始

```python
bicycles = ['trek', 'cannondale', 'redline', 'specialized']
print(bicycles[0])                #访问第一个元素
print(bicycles[-1])                #访问最后一个元素 -2 ……以此类推
```

### 修改、添加和删除

```python
motorcycles = ['honda', 'yamaha', 'suzuki']
motorcycles.append('ducati')                #在列表末尾添加元素
motorcycles.insert(0, 'ducati')            #插入，指定索引和值，其他相应右移
del motorcycles[0]                                    #删除0元素
```

使用方法pop()删除元素

```python
motorcycles = ['honda', 'yamaha', 'suzuki']
popped_motorcycle = motorcycles.pop()                #弹出列表最后一项，赋给变量
first_owned = motorcycles.pop(0)                        #添加参数，弹出任意位置
```

根据值删除元素

```python
motorcycles = ['honda', 'yamaha', 'suzuki']
motorcycles.remove('ducati')                #删除列表中值为给定的一项
```

### 排序、打印和确定长度

```python
cars = ['bmw', 'audi', 'toyota', 'subaru']
#永久排序 sort()
cars.sort()                                        #按字母表顺序，永久性排序
cars.sort(reverse=True)                #反序

#临时排序 sorted(cars)
print(sorted(cars))
```







