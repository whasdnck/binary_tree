# 이진 트리(binary tree) 란?
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
# 이진 탐색 트리(Binary Search Tree) 란?
### 왼쪽 자식은 부모보다 작고 오른쪽 자식은 부모보다 큰 이진 트리이다.
# 조건
### 1) 부모 노드의 왼쪽 노드는 부모 노드보다 작아야 한다.
### 2) 부모 노드의 오른쪽 노드는 부모 노드보다 커야 한다.

### 전위 순회(preorder traverse) : 뿌리(root)를 먼저 방문
### 뿌리 -> 왼쪽 자식 -> 오른쪽 자식
### ( 8 -> 1 -> 3 -> 6 -> 4 -> 7 ....)
### 중위 순회(inorder traverse) : 왼쪽 하위 트리를 방문 후 뿌리(root)를 방문
### 왼쪽자식 -> 뿌리 -> 오른쪽 자식
### ( 1 -> 3 -> 4 -> 6 -> 7 -> 8 -> ...)
### 후위 순회(postorder traverse) : 하위 트리 모두 방문 후 뿌리(root)를 방문
### 왼쪽자식-> 오른쪽 자식 -> 뿌리
### (1 -> 4 -> 7 -> 6 -> 3 -> 13 -> ..)
![image](https://user-images.githubusercontent.com/127116197/227396280-b603019c-6760-4db6-be28-f88378eb3eb0.png)

# 정 이진 트리(full binary tree) 란?
### 모든 노드가 0개 또는 2개의 자식 노드를 갖는 트리이다.
![image (1)](https://user-images.githubusercontent.com/127116197/227396359-dd91a458-02d1-4409-aa68-db1e09b57005.png)
# 완전 이진 트리(complete binary tree) 란?
### 마지막 레벨을 제외하고 모든 레벨이 완전히 채워져 있는 트리이다.
![image (2)](https://user-images.githubusercontent.com/127116197/227396460-53359031-90bd-47b4-9693-8a46ec831bec.png)

# 완전 이진 탐색 트리(Complete binary search tree)란?
### 완전 이진 트리의 성질을 가지는 이진 탐색 트리이다.
### 편향된 이진 탐색 트리와 다르게 항상 O(log n)의 검색 속도를 보장한다.
### 하지만 트리에 자료가 삽입될 때 마다 완전 이진 탐색 트리의 형태를 유지하기 위해
### 트리의 모양을 바꾸어야 하기 때문에 삽입 시 시간이 많이 소요된다.
![image (3)](https://user-images.githubusercontent.com/127116197/227396769-109686fe-7d8e-4981-ba38-770d291a64bb.png)

# 포화 이진 트리 (Perfect Binary Tree)란?
### 정 이진 트리이면서 완전 이진 트리인 경우이다.
### 모든 리프 노드의 레벨이 동일하고, 모든 레벨이 가득 채워져 있는 트리이다.
### 즉, 모든 노드가 두 개의 자식 노드를 가지며 모든 잎 노드가 동일한 깊이 또는 레벨을 갖는다.
### 따라서 삽입이 적고 탐색이 많은 경우에 유리하며,
### 삽입하는 빈도수가 높아지면 효율성이 떨어지고 이를 해결한 것이 AVL트리이다.
![image (4)](https://user-images.githubusercontent.com/127116197/227396952-aebfb5a1-32f8-47b3-8b04-7643827b301c.png)

# 편향 이진트리(skewed binary tree)란?
### 같은 높이의 이진 트리 중에서 최소 개수의 노드 개수를 가지면서
### 왼쪽 혹은 오른쪽 서브트리만을 가지는 이진트리이다.
### 즉 모든 노드가 왼쪽에 있거나 반대로 오른쪽에 있는 트리이다.
### 각 부모 노드가 오직 한 개의 연관 자식 노드를 갖는 트리이다.
### 사향 이진 트리(Degenerate (or Pathological) Tree) 라고도 부른다.
### Linked List 성능과 동일하다.
![image (5)](https://user-images.githubusercontent.com/127116197/227397111-57f4de0d-0ccf-4624-bb95-1c75a3274ed5.png)

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
