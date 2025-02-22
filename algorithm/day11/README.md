# 오늘의 학습 

- [문제 링크 - 백준 1461](https://www.acmicpc.net/problem/1461)

### 그리디

- 주어진 문제는 그리디이다. 
  - 그리디를 푸는 이상적인 흐름은 다음과 같다고 한다. 
    1. 관찰을 통해 탐색 범위를 줄이는 방법을 고안한다. 
    2. 탐색 범위를 줄여도 올바른 결과를 낸다는 사실을 수학적으로 증명한다. 
    3. 구현해서 문제를 통과한다. 

<br>

### 오늘의 회고
  - 어떤 문제가 있었고, 나는 어떤 시도를 했는지 
    - 이분 탐색과 관련한 문제를 풀었다. 
    - 이분 탐색으로 문제를 풀려고 했다. 

  - 어떻게 해결했는지 
    - 처음에는 투포인터로 풀어야 하는 문제인 줄 알았다. (정렬을 하고 양쪽 끝에서부터 비교하면 되지 않을까...?)
    - 하지만, 문제를 풀면서 음수와 양수를 나누지 않고 푸니, 효율적으로 풀고 있지 못하다는 생각이 들어서 작성하고 있던 코드를 지우고 문제를 보면서 다시 생각을 했다. 
    - 투포인터처럼 비슷하게 풀어야 할 것 같은데, 음수와 양수를 나누어서 풀 수 있는 방법이 어떤 것이 있을까 생각했을 때, 우선 순위 큐를 사용하면 정렬도 따로 해주지 않아도 될 것 같아서 2개의 우선 순위 큐를 사용해서 풀었다. 
    - 여기서 걷는 거리를 계산할 때 중요한 것은 계산은 일괄적으로 2배를 곱해주는 식으로 계산을 하다가 마지막에 제일 먼 거리를 빼주는 것이다. (제일 먼 거리는 왕복이 아닌 1번만 가게 하는 것이 더 짧기 때문)

  - 무엇을 새롭게 알았는지
    - 양수와 음수를 나누어서 풀어야 하는 것이 문제의 핵심이라는 것을 알게 되었다. 

<br>

> [다음의 글을 참고하였습니다.](https://blog.encrypted.gg/975)