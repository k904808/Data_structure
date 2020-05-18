# 정렬(Sorting)

#### 정렬(Sorting)이란?
어떤 데이터들이 주어졌을 때 이를 정해진 순서대로 나열하는 것

정렬은 프로그램 작성 시 빈번하게 필요로 함
다양한 알고리즘이 고안되었으며, 알고리즘 학습의 필수

#### 버블 정렬(bubble sort)이란?

 인접한 두 데이터를 비교해서 앞에 있는 데이터가 뒤에 있는 데이터보다 크면 자리를 바꾸는 정렬 알고리즘.

```
for i in range(len(data)-1):
    for j in range(len(data) -i -1):
        if data[j] > data[j + 1] :
            data[j], data[j + 1] = data[j + 1], data[j]
```
