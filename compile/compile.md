# 编译原理学习

## 编译步骤

- 词法分析
  - 解析关键字
- 语法分析
  - 构造语法树树
- 语义分析
  - 类型检查
- 中间代码
- 代码优化
- 目标机器代码

## 词法分析

### 识别器

- 可以在字节流中识别单词
- 有限状态自动机
- 状态转移图

### 正则表达式

- 选择
  - a|b
- 连接
  - a{b|c}
- 闭包
  - a*
- grep
  - <u>global</u> <u>regular</u> <u>expression</u> <u>pattern</u> match and print的缩写

### NFA（不确定性有限自动机）

### DFA（确定性有限自动机）

### 词法分析器

- 会过度读取，然后再回滚

## 语法分析

根据词法分析的出的单词流，构建语言中的一个完整语句

### 上下文无关语法

- 为何不使用正则表达式
  - 无法理解算数优先级
  - 可以匹配不正确的语法
- 产生式
  - 非终结符号：产生式中的语法变量
  - 终结符号：被推导出来的语句中的单词
- 句型：有效推导中`终结符号`和`非终结符号`的集合

## 语义分析

### 检查类型是否能正确计算

- 强类型语言：每个表达式分配到无歧义的类型
- 静态类型：表达式在编译时确定类型
- 反之则是弱类型和动态类型

## 中间表示

### 符号表

- 分作用域的符号表
- 记录信息

