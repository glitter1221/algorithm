# Graph

그래프(Graph)는 정점(Vertex)의 집합 V와 간선(Edge)의 집합 E로 구성된 비선형 데이터 구조이다.

Vertex : 자료를 저장하려는 자료의 단위, 노드(Node)라고도 말함.

Edge : 정점 사이를 연결하는 선으로 두 정점 쌍 (u, v)로 표현함.

G = (V , E)



![graph1](./images/graph1-min.JPG)



G1과 G2는 무방향 그래프, G3는 방향 그래프를 의미한다.

V(G1) = {1, 2, 3, 4}
E(G1) = {(1, 2), (1, 3), (1, 4), (2, 3), (2, 4), (3, 4)}

V(G2) = {1, 2, 3, 4, 5, 6, 7}
E(G2) = {(1, 2), (1, 3), (2, 4), (2, 5), (3, 6), (3, 7)}

V(G3) = {1, 2, 3}
E(G3) = {(1, 2), (2, 1), (2, 3)}



![graph2](./images/graph2-min.JPG)



adjacent : 무방향성 그래프에서 정점 u, v에 대하여 간선(u, v)가 있으면 정점 u는 정점 v에 인접(adjacent)하다고 한다.(v는 u에 대한 역도 성립)
 방향성 그래프에서 정점 u, v에 대하여 간선(u, v)가 있으면 정점 u는 정점 v에 인접(adjacent)하다고 한다.(v는 u에 대한 역은 성립하지 않음)

incident : 무방향 그래프에서 정점 u, v에 대하여 간선(u, v)이 있으면 간선(u, v)은 정점 u와 v에 부속(incident)한다고 한다.



![graph3](./images/graph3-min.JPG)



self-loop : 한 간선이 같은 정점에 부속(incident)해 있을 때 self-loop라고 한다. e = (u, u)

isolated : 간선이 없는 정점을 isolated vertex라고 한다.