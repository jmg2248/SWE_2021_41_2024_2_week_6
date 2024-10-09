# SWE_2021_41_2024_2_week_6

---

## Week 4 Assignment
https://github.com/jmg2248/SWE_2021_41_2024_2_week_4.git

```python
def isHappy(n):
  lst=[]
  while(1):
    sum=0
    while(n):
      i=n%10
      i=i**2
      sum+=i
      n=n//10
    if sum==1:
      return True
    else:
      n=sum
      lst.append(n)
      if lst.count(n)>1:
        return False
      else:
        pass
```

description\

---

## Week 5 Assignment
> ```console docker exec <your container> cat /etc/os-release ``` \
> explain

> docker exec <your container> git --version \
> explain

> docker exec <your container> python3 --version \
> explain

> docker inspect --format="{{ .HostConfig.Binds }}" <container_name> \
> explain
