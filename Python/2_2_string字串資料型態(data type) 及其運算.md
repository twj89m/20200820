# string字串 資料型態(data type) 及其運算
```
[1]string字串 資料型態(data type) 
[2]string字串的運算
[3]Python内建的字串函数(Built-in String Methods)
```
# [1]string字串 資料型態(data type) 
```
Python 字串資料型態 (str) 

變數值以一對雙引號 (「"」)或單引號 (「'」)
```
```
str1 = '這是字串'
print(str1)

str2 = "這也是字串"
print(str2)

str3 = 'allows embedded "double" quotes'
print(str3)
```
# [2]string字串的運算

### 存取字串中的值: 使用方括號
```
#!/usr/bin/python
 
var1 = 'Hello Python!'
 
print("var1[0]: ", var1[0])
print("var1[1:8]: ", var1[1:8])
```
### 字串的更新 
```
#!/usr/bin/python
# -*- coding: UTF-8 -*-
 
str1 = 'Hello World!'

print("更新前的字串-> ", str1[:])
print("更新前的字串(也可以這樣寫)-> ", str1)
print("更新後的字串-> ", str1[:6] + 'Python!')
```

### 字串的加法運算
```
str4=str1 + str2
print(str4)
```
###  更多練習
```
a='  Hello   '
b='  Python ! '

a+b

a*2

a[1:4]

"H" in a

"H" not in a
```
# 字串反轉
```
Reverse string in Python (5 different ways)

https://www.geeksforgeeks.org/reverse-string-python-5-different-ways/
```
```
def reverse(s): 
    if len(s) == 0: 
        return s 
    else: 
        return reverse(s[1:]) + s[0] 
  
#s = "HappyHackingDay"
s = "BreakAllCTF{HappyHackingDay}"

print ("The original string  is : ",end="") 
print (s) 
  
print ("The reversed string(using recursion) is : ",end="") 
print (reverse(s))
```
# [3]Python内建的字串函数(Built-in String Methods)
```
底下以幾個常見的示範

更多的練習請參考底下

https://www.tutorialspoint.com/python/python_strings.htm
```
```
str1='happy python day'
str2='    Oh!   '
str4=str1 + str2
print(str4.capitalize())
```
```
mystr = 'python'
str4.find(pyth, beg=0, end=len(str4))
```
```
print(str4.encode('base64'))
```
### isalpha() :檢測字串是否只由字母組成
```
#!/usr/bin/python
# -*- coding: UTF-8 -*-
 
str = "Python2019"
print(str.isalpha())

str = "Python"
print(str.isalpha())
```
###  isalnum():檢測字串是否由字母和數位組成。
```
如果 string 至少有一個字元並且所有字元都是字母或數字則返回 True,
否則返回 False
```
```
#!/usr/bin/python
# -*- coding: UTF-8 -*-
 
str = "Python2019"
print(str.isalnum())

str = "Python"
print(str.isalnum())

str = "2019"
print(str.isalnum())

str = "Python 2019"
print(str.isalnum())
```
