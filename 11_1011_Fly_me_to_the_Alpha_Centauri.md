## 나의풀이
- 1트실패
- 배열을 만들어 내고 규칙을 찾아냈지만 코드로 만들어내는데 실패
## 다른풀이 1

<pre>
<code>



import math

t = int(input())

for _ in range(t):
    x,y = map(int, input().split())
    distance = y - x
    if distance <= 3:
        print(distance)
    else:
        n = int(math.sqrt(distance))
        if distance == n**2:
            print(2*n-1)
        elif n**2< distance <= n**2 + n:
            print(2*n)
        else:
            print(2*n + 1)
</code>
</pre>





- 나랑은 다른 규칙을 코드로 구현해냄
- 간결하고 직관적임
- https://wookcode.tistory.com/35
