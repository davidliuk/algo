# 优化

- 减治：无效优化

  避免无效计算：不可能出现答案的地方直接排除，即优化无效状态空间

  有序（广义上的有序，符合一定的规律）的线性结构

  （四大类型）eg. 二分法，快速选择

- 动归：重叠优化

  避免重复计算：

  DAG结构

  复杂的动态规划可以把四种算法都串起来，因为临界节点的序列是线性的，且有的时候是“有序”的，就可以减治（如斜率优化等）



动态规划的优化

- 空间优化：

  先序：

  - FOR：滚动数组
  - DFS、BFS：把hashmap的节点删除（hashmap.remove）

  后序：

  - 只有被重复计算的点需要被存储下来，没有重复计算的点就不需要存储
  - lc一道hard里面出现过一次

- 时间优化：通过减治



