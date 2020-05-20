# 큐(Queue)

#### 1. 큐 구조
가장 먼저 넣은 데이터를 가장 먼저 꺼낼 수 있는 구조. 
줄을 서는 행위와 유사.

>- 스택과 꺼내는 순서가 반대
FIFO (First In First Out)
LILO (Last In Last Out)

#### 2. 알아둘 용어
Enqueue : 큐에 데이터를 넣는 기능
Dequeue : 큐에서 데이터를 꺼내는 기능

#### 3. 파이썬 queue 라이브러리 활용해서 큐 자료구조 사용하기
- Queue() : 가장 일반적인 큐 자료구조
- Lifo  Queue() : 나중에 입력된 데이터가 먼저 출력 (스택구조)
- Priority Queue() : 데이터마다 우선순위를 넣어서, 우선순위가 높은 순으로 데이터 출력

```
import queue
test = queue.Queue()
test.put()
test.size()
test.get()

test = queue.LifoQueue()
test.put()
test.size()
test.get()

test = queue.PriorityQueue()
test.put((10, a))             # 튜플로 우선순위와 데이터를 함께 넣는다
test.put((1, b))              # 숫자가 낮을수록 우선순위가 높은 것!
```
#### 4. 큐가 어디에 많이 쓰이나?
멀티태스킹을 위한 프로세스 스케줄링 방식을 구현하기 위해 많이 사용됨.v
