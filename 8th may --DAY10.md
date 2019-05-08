
## Printing statement


```python
print('hello world')
```

    hello world
    

## variable assignment


```python
var1=4
var2=var1**var1
var3=var1*var2
print(var1,"  ",var2," ",var3)

```

    4    256   1024
    

## count digits in a number


```python
print(len(str(var3)))
```

    4
    

## Getting the datatype of a variable


```python
var3="dff"
type(var3)
```




    str




```python
type(var1)
```




    int



## String slicing


```python
str1="python programming"

str1[0]##printing the 1st character
```




    'p'




```python
str1[4]

```




    'o'




```python
str1[2:]
```




    'thon programming'




```python
str1[1:8] ##printing from 1 to 7 characters
```




    'ython p'




```python
str1[len(str1)-1]##accessing the lst character
```




    'g'




```python
str1[0:6] ##printing 1st 6 characters
```




    'python'




```python
str1[:6] ##printing 1st 6 characters
```




    'python'




```python
str1[len(str1)-1::-1]  ## Reverse of a string
```




    'gnimmargorp nohtyp'




```python
str1[::2]
```




    'pto rgamn'




```python
str1[5::-2]
```




    'nhy'




```python
str1[7:] * 10
```




    'programmingprogrammingprogrammingprogrammingprogrammingprogrammingprogrammingprogrammingprogrammingprogramming'



## List   --  Mutable     



```python
lii=[12, "string" , 9.76] #indexing starts from 0

lii
```




    [12, 'string', 9.76]




```python
len(lii) ## length of the list
```




    3




```python
lii[1] ## accessing a single element in the list
```




    'string'




```python
lii[2]='programming' ## replacing the existing element in the list
lii
```




    [12, 'string', 'programming']




```python
lii.append('python') ## to add ta element to the list
lii
```




    [12, 'string', 'programming', 'python']




```python
lii.pop()
```




    'python'




```python
lii
```




    [12, 'string', 'programming']




```python
lii.pop() ## pop without any index used to remove element at the end of the list
```




    'programming'




```python
lii
```




    [12, 'string']




```python
lii.remove(12) ## remove romoves the element using value
```




    ['string']




```python
lii.append('programming')
lii
```




    ['string', 'programming', 'programming']




```python
lii.append(123) ## add the new element to the end of the string
lii
```




    ['string', 'programming', 'programming', 123]




```python
lii.pop(2) ## pop removes the element using index
```




    'programming'




```python
lii
```




    ['string', 'programming', 123]




```python
lii.insert(1,76)
li
```




    ['string', 76, 76, 'programming', 123]




```python
lii.insert(2,'asd') ## add elements at a particular position
lii
```




    ['string', 76, 'asd', 76, 'programming', 123]




```python
li2=[[1,2,3],[4,5,6],[7,8,9]] ## multi dimensional list
li2
```




    [[1, 2, 3], [4, 5, 6], [7, 8, 9]]




```python
li2[1] #accessing a single list in multi dimensional list
```




    [4, 5, 6]




```python
li2[1][0] #accessing a single element in a list in multi dimensional list
```




    4




```python
li2.insert(3,[10,11,12])
```


```python
li2
```




    [[1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11, 12]]




```python
li2.pop(2)
```




    [7, 8, 9]




```python
li2
```




    [[1, 2, 3], [4, 5, 6], [10, 11, 12]]




```python
li2[1].pop(1)
```




    5




```python
li2
```




    [[1, 2, 3], [4, 6], [10, 11, 12]]




```python
li2[1].insert(2,7)
```


```python
li2
```




    [[1, 2, 3], [4, 6, 7], [10, 11, 12]]




```python
for i in range(0,len(li2)):
    for j in range(0,len(li2[i])):
        print(li2[i][j] ,end=' ')
```

    1 2 3 4 6 7 10 11 12 


```python
for i in range(len(li2)-1,-1,-1):
    for j in range(len(li2[i])-1,-1,-1):
        print(li2[i][j] ,end=' ')
```

    12 11 10 7 6 4 3 2 1 

## TUPLE --- immutable[ cannot be changed]


```python
t1=(12,13,14)
```


```python
t1[1]
```




    13




```python
t1[2]
```




    14




```python
t1[1]+t1[2]
```




    27




```python
t1[len(t1)-1]
```




    14




```python
t1[1:3]
```




    (13, 14)




```python
t1
```




    (12, 13, 14)




```python
str(t1[0])[1]+ "  " +str(t1[1])[1]+"  "+str(t1[2])[1]
```




    '2  3  4'



### PROBLEM 1:
#### Problem statement:
* For a given number check If it is divisible by 2 and 3 but not 4

#### Constraints-
* given number will be In the Range [1,1000000000]

#### Test cases:
* checkDivisibility(6) -> True
* checkDivisibility(16) -> False
* checkDivisibility(20) -> False


```python
def checkDivisibility(n):
    if n%2 ==0 and n%3 == 0 and n % 4 !=0:
        return True
    else:
        return False
    
    
checkDivisibility(4)
```




    False




```python

```


```python

```
