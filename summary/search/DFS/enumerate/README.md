# 枚举：宽树搜索

枚举类问题的特点：

1. 深度线性

   解空间的深度小于等于传入序列的长度

   故栈空间占用始终是线性可解的

2. 宽度指数

   解空间的宽度呈现指数级别增长

   每个节点可以扩散0-n个

搜索

## 简单枚举

xxx

## 排列枚举

### 序列全排列



### 下一个排列

## 子集枚举

从代码量看，枚举子集的最简单方法是二进制法

### 增量构造法

需要使用定序的技巧，避免同一个集合枚举多次

### 位向量法

解答树的节点略多，但是大多数情况下也足够使用

### 二进制法

二进制表达子集S，从右往左第i位（从0开始编号），表示元素i是否在集合S中（0为不在，1为在）

二进制集合的运算，交并对称差：`&|^`

```java
for (int s = 0; s < (1 << n); s++) {
    printSubset(s);
}
```
