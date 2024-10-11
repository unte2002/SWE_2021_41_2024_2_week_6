# unte2002-SWE_2021_41_2024_1_week_6
---
## Week 4 assignment

__unordered list__
- Link of my repository\
[Assignment 4](https://github.com/unte2002/SWE_2021_41_2024_1_week_4)
```python
def isHappy(n):
  num = n
  checkLoop = []
  while 1:
    digits = []
    while num>0:
      digits.append(num%10)
      num = int(num/10)
    for k in digits:
      num = num+ k*k
    if num == 1:
      return True
    else:
      for j in checkLoop:
        if j==num:
          return False
      checkLoop.append(num)
```
- Description of my code\
**Basically the function "isHappy" takes number n as an input and returns True if the number satisfies specific property and False if it doesn't.**

---
## Week 5 assignment
> <code>docker exec <your container> cat /etc/os-release</code>\
*The command retrieves and displays the operating system information from the /etc/os-release file inside a running Docker container.*

> <code>docker exec <your container> git --version</code>\
*The command checks the version of Git installed in a running Docker container by executing git --version inside it.*

> <code>docker exec <your container> python3 --version</code>\
*The command checks the version of python installed in a running Docker container by executing it --version inside it.*
