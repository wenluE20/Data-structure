# 图的属性
**实验内容**

(1) 判断车站的路线图是否连通。从一个顶点开始遍历，如果能遍历到所有站点，那么图连通。

(2) 计算图中节点的度（degree）。

*节点度，是指和该站点相关联的边的条数。*

(3) 计算图的聚类系数（clustering coefficient）。

*点的聚类系数是所有与它相连的顶点之间所连的边的数量，除以这些顶点之间可以连出的最大边数。图的聚类系数是所有点的聚类系数的均值*。

(4) 若图连通，使用Dijkstra算法计算从某个站点到另一站点的最小票价。

(5) 若图连通，计算图的直径（diameter），半径（radius）。定义如下：

*节点距离：指的是两个节点间的最短路径的长度。*

  *Eccentricity：这个参数描述的是从任意一个节点，到达其他节点的最大距离*

  *Diameter：图中的最大的Eccentricity*

  *Radius：图中的最小的Eccentricity*
  

**输入：**

7        // 节点数

8        // 节点相邻边数

0 6 1  ////节点0到节点6有一条长度为1的边

1 6 2

1 2 3

2 3 4

3 4 5

4 6 6

4 5 7

1 3 8

**输出：**

connected: 1

degree distribution:

node0:1,node1:3,node2:2,node3:3,node4:3,node5:1,node6:3,

clustering coefficient:0.238095

the minimum fare between 1 and 3: 7

Path: 1->2->3

diameter:16

radius:9
