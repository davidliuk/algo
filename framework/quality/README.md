# 代码质量

也称 Coding Style

优化的逻辑：

1. 先想暴力的方法
2. 看哪里有地方是浪费的

#### 优秀的 Coding Quality

1. bug free

2. 有边界检测和异常处理

3. 代码风格：命名规范、空格、空行

   1. 每一个逻辑 Part 之间一个空行划分

      如异常判断、主体逻辑、结果返回，这些part之间一个分行

   2. 变量命名：全称，1-2个单词，小驼峰

   3. 避免重复代码

      泄露没有工程经验

   4. 用不到的变量用_来命名

   5. 尽可能避免全局变量

   6. 缩进

      1. java是4个
   
   7. 空格
   
      1. 运算符前后要有
      2. 逗号、分号后面有

> 写Python能大概减少10分钟的时间，如果是面试不限制语言的话，可以写Python

### 独孤九剑 - 总决式

想做到 bug free 最重要的是优化code Quality

单元运算符：--, ++, !

多用 continue 少用 else：减少大段代码的缩进

减少 else，如果前面的if里面执行了return或者continue、break等，后面就不需要else if，直接普通的if，最后不需要else，直接普通的xxx

最好把嵌套式的改成并列的：好懂得多

减少typo：拼写错误