# Tree

트리란 노드들이 나무 가지처럼 연결되어 있는 비선형 계층적 자료구조이다.



![tree1](./images/tree1-min.JPG)



node : 트리를 구성하고 있는 기본 요소인 데이터

edge : 노드와 노드 간의 연결선

root node : 트리 구조에서 부모가 없는 최상위 노드

parent node : 자식 노드를 가진 노드

child node : 부모 노드의 하위 노드

sibling node : 같은 부모를 가지는 노드

external node, outer node, leaf node : 자식 노드가 없는 노드

internal node, inner node, branch node : 자식 노드를 하나 이상 가진 노드

depth : 루트에서 어떤 노드까지의 간선(edge)의 수

height : 어떤 노드에서 리프 노드까지 가장 긴 경로의 간선(edge) 수



![tree2](./images/tree2-min.JPG)



level : 루트에서 어떤 노드까지의 간선(edge) 수

degree : 노드의 자식 수

path : 한 노드에서 다른 한 노드에 이르는 길 사이에 놓인 노드들의 순서

path length : 해당 경로에 있는 노드들의 총합

size : 자신을 포함한 자손의 노드 수

width : 레벨에 있는 노드 수

breadth : 리프 노드의 수

distance : 두 노드 사이의 최단 경로에 있는 간선(edge)의 수

order : 자식 노드 중 가장 많은 자식을 가진 노드의 자식 노드 개수


트리의 운행(traversal)이라고 하는 것은 트리의 각 노드를 중복되지 않게 한 번씩 방문하여 트리의 정보를 검색하는 것으로써 순방, 순회 또는 순행이라고 한다.
일반적으로 전위(preorder), 중위(inorder), 후위(postorder) 운행 방법이 있다.



![tree3](./images/tree3-min.JPG)



전위(preorder) 운행법은 루트 노드를 먼저 방문하고, 그 서브 트리에 대하여 왼쪽 노드에서 오른쪽 노드로 방문하기를 되풀이하는 것이다.
A, (T1), (T2)
 = A, B, D, (T11), C, F, (T22)
 = A, B, D, E, H, C, F, G, I, J


중위(inorder) 운행법은 왼쪽 서브 트리를 먼저 방문한 후 루트 노드를 방문하고, 오른쪽 서브 트리를 방문하는 방법이다.
(T1), A, (T2)
 = D, B, (T11), A, F, C, (T22)
 = D, B, H, E, A, F, C, I, G, J


후위(postorder) 운행법은 왼쪽 서브 트리를 먼저 방문한 후 
(T1), (T2), A
 = D, (T11), B, F, (T22), C, A
 = D, H, E, B, F, I, J, G, C, A

