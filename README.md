# CUB3D
## Description
> This project is inspired by the world-famous eponymous 90's game, which was the first FPS ever. It will enable you to explore ray-casting. Your goal will be to make a dynamic view inside a maze, in which you'll have to find your way.

### 레이캐스팅
> 가상의 공간에 보이지않는 빛(ray)을 투사해 빛에 닿는 표면을 파악하는 기술
+ 레이캐스팅은 2차원 맵에서 3차원의 원근감을 만드는 렌더링 기술
  + 레이캐스팅은 스크린의 모든 수직선에 대해 계산만 하면 되어서 속도가 빠르다.
  + 컴퓨터가 지금보다 느려서 3D 엔진을 실시간으로 실행 할 수 없던 과거에는 레이캐스팅이 최초의 해결이었다.

### DDA(digital Differential Analysis)
+ DDA알고리즘은 2차원 그리드를 지나가는 선이 어떤 네모칸과 부딪히는지 찾을때 일반적으로 사용되는, 속도가 빠른 알고리즘이다.
+ 이 알고리즘을 사용해서 광선이 맵에서 어떤 네모칸이랑 부딪히는지 찾아낼 수 있고, 벽에 부딪힌 것이 확인되면 이 알고리즘은 중단된다.

### vector
+ 플레이어의 위치는 항상 벡터(x좌표, y좌표)이다.
  + 플레이어가 보는 방향으로 선을 그릴경우, 그 선위의 모든 점들은 ‘플레이어의 위치 + 방향 벡터의 배수’ 의 합이다.
  + 방향벡터의 방향만 중요하고 길이는 크게 중요하지 않다. x랑 y에 같은 값을 곱하면 길이는 바뀌더라도 같은 방향을 나타낸다.
