# 递归

啥是递归？

当函数直接或者间接调用自己时，则发生了递归

递归的定义：参见“递归的定义”

---

递归的三要素

- 递归的定义 (接收什么参数, 返回什么值, 代表什么含义)

- 递归的拆解 (把大问题拆解成小问题)（或者叫转移）

- 递归的出口 (到什么时候结束)


---

迭代形式与递归形式比较

时间复杂度：迭代O(n), 递归O(n)

空间复杂度：迭代O(1), 递归O(n)

递归的O(n)空间是栈空间 or 堆空间？

---

### 内存中的堆和栈

堆空间

- 存放 new 得到的对象
- 无限制 (剩余内存的大小)

栈空间

- 存放对象的引用
- 值类型变量
- C++函数中的数组
- 有限制, 一般很小, MB量级
- 函数调用栈

函数调用栈

想象一个“圆筒”，调用的函数需要放到筒里

第一个进入“圆筒”的是main函数

每发生一次新的函数调用，就会有一个新函数进入“圆筒”

正在执行的就是最上面的函数

一个函数执行完毕，就会被拿出来

圆筒满了怎么办？

N 如果过大，有可能还没来得及从圆筒中拿出函数圆筒就满了

递归需谨慎

递归调用容易爆栈

人为调用栈不会爆栈

除非在C/C++的函数中定义大数组——危险行为