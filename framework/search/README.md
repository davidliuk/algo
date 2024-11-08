# 搜索

搜索的分类：

- FOR 循环
- DFS 深搜
- BFS 广搜

## 对比

### DFS对BFS优势

1. 后序传值

   DFS专属后序位置，可以让父收到子传的值

2. 先序回溯

   DFS优点，可以节省空间

3. 宽树搜索

   空间复杂度对比：

   BFS：树的最大宽度

   DFS：树的最大深度

   宽树搜索，必须DFS

也就是说在这两种特定场景下只能用DFS。那既然BFS这么弱，我们还要BFS有什么用呢？请问何种数据结构的搜索必须要BFS呢？BFS的搜索过程不像DFS，DFS的栈对使用者是不可见的，但BFS的队列却是可见的，请问这种可见性带来了什么样的好处，请谈谈你的想法？

### BFS对DFS优势

1. 最短路径
2. 拓扑排序

---

1. 请问根据你所实现栈模拟代码，谈一下为什么编程语言要有递归这个功能，如果没有麻烦的点在哪里？

   如果显示的实现递归，需要手动模拟栈来维护每个状态节点的信息，较为繁琐，编程语言实现的递归有利于简化操作。
   
2. 为什么DFS是运行时栈，而BFS是等待队列呢？
	
	DFS：运行时栈 → 入栈代表开始执行，出栈代表执行完毕  → 先序（入栈） + 后序（出栈）
	
	BFS：等待队列 → 入队代表已经访问完毕，出队代表开始扩展邻接  → 先序
	
3. 为什么DFS支持先序和后序、而BFS仅支持先序？
	
	DFS的入栈顺序可以进行先序传值，DFS的出栈时候可以进行后序传值
	
	BFS只有在出队的时候进行传值
