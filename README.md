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

__Description of my code__
1. while(n) 안에서 이번의 수가 각 자릿수의 제곱의 합이 1인지 파악한다. 
2. 만약 제곱의 합이 1이라면 happy number의 조건을 만족하므로 True를 return하고 끝이 난다. 
3. 1이 아니라면 나온 합을 lst에 집어넣고 지금까지 lst에 이 합이 나온적이 있는지 확인한다. 
(확인은 해당 값 n이 lst 몇개 있는지 count(n)을 통해 확인함) 
4. 만약 이전에 이 합이 나온적이 있다면 해당 수는 cycle을 돌고 있는 것이므로 False를 return, 이외에 경우에는 다시 해당 과정을 반복하면서 1이 나올 수 있는지 확인한다. 

---

## Week 5 Assignment
> ```shell
> docker exec <your container> cat /etc/os-release
> ```
> 현재 내 container에 우분투가 제대로 설치되어있는지 확인

> ```shell
> docker exec <your container> git --version
> ```
> 현재 내 container에 git이 제대로 설치되어있는지 확인

> ```shell
> docker exec <your container> python3 --version
> ```
> 현재 내 container에 python3가 제대로 설치되어있는지 확인

> ```shell
> docker inspect --format="{{ .HostConfig.Binds }}" <container_name>
> ```
> 현재 내 container에 bind mount가 제대로 되어있는지 확인

<img src="./2020311661_week5.png" title="Screenshot"/>

과제의 요구사항을 제대로 수행했을 시 다음과 같은 스크린샷을 볼 수 있다.
