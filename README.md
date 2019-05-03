# SOME ALGOS IN PYTHON NOT FOUND GEEKS FOR GEEKS
some algorithms not found in geeks for geeks in python or a moer efficient way in python two implement the algorithms

# 1) Count factors of two numbers

Input:
```
10 15
```
Output:
```
2
```
```
import math

def gcd(a, b) :
    if (a == 0) :
        return b
    return gcd(b%a, a)
    
def commDiv( a, b) :

    n = gcd(a, b)
    result = 0
    for i in range(1,math.floor(math.sqrt(n))+1): 
        if (n%i==0) :
            if (n/i == i) :
                result += 1
            else:
                result += 2

    return result

# Write your code here
a,b=map(int,input().strip().split(' '))
print(commDiv(a,b)) 

```
