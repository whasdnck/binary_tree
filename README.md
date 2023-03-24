# 이진 탐색 트리 란?
### 각각의 노드가 최대 두 개의 자식 노드를 가지는 트리 자료 구조 로,
### 자식 노드를 각각 왼쪽 자식 노드 와 오른쪽 자식 노드 라고 한다.
### 이진 탐색 트리에서 root 노드를 기준으로 왼쪽 서브트리의 가장 왼쪽 값이 트리에서 가장 작은 값,
### 오른쪽 서브트리의 가장 오른쪽 값이 트리에서 가장 큰 값이 된다.
### 또한 왼쪽 서브트리의 가장 오른쪽 값이 root 값 보다 작은 값들 중 가장 큰 값이 되며,
### 오른쪽 서브트리의 가장 왼쪽 값이 root 값 보다 큰 값들 중 가장 작은 값이 된다

![images_vermonter_post_ce30fa04-f438-4557-bb99-553a7fc93726_image](https://user-images.githubusercontent.com/127116197/227128899-c3b78754-6fbd-47bd-8179-1967f1606dbe.png)

# 이진 트리 연산
### 1. 찾고자 하는 값과 root 값을 비교한다.
### 2. 찾고자 하는 값이 root 값보다 작을 경우 왼쪽 서브트리에서, 클 경우 오른쪽 서브트리에서 탐색한다.
### 3. 찾고자 하는 값을 찾을 때까지 반복한다.
### 4. 만일 찾고자 하는 값이 없다면 null을 반환한다.
![images_hanif_post_26177041-2135-4c3c-81fe-bacbe2dac2cc_image](https://user-images.githubusercontent.com/127116197/227130998-b0815217-4522-4189-925b-f29793879015.png)

# "트리"의 개념
### 1. 트리는 하나의 루트 노드를 갖는다.
### 2. 루트 노드는 0개 이상의 자식 노드를 갖는다.
### 3. 자식 노드 또한 0개 이상의 자식 노드를 갖는다.
### 4. 노드(Node)들과 노드들을 연결하는 간선(Edge)들로 구성되어 있다.
# "Left, Right" 설명
### 모두 유일한(중복되지 않는) 키 값을 가진다.
### 왼쪽과 오른쪽의 서브트리도 이진트리여야 한다.
### 노드의 왼쪽 서브트리는 루트의 키보다 작은 값을 가진다.
### 노드의 오른쪽 서브트리는 루트의 키보다 큰 값을 가진다.
![dkssudgktpdyz](https://user-images.githubusercontent.com/127116197/227129866-675ca133-a089-48f6-9491-a6575a68f24d.png)
# Left, Right Full Code
![화면 캡처 2023-03-23 162731](https://user-images.githubusercontent.com/127116197/227132947-2e36a356-a484-4590-b776-2a7d106d2a80.png)
