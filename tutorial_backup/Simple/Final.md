# 图解 Final,final 的功能

## 话不多说，先上逻辑图

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Final_example.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 如果本地规则匹配成功，则会往下走，不会往右边走

## 还不懂就再理解下图

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Final_example_1.png)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 逻辑对应关系如下图所示

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Final_example_2.jpg)

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) 上图中因为本地规则中没有匹配成功，就不往下走而是往右边走

## 实例完成一次访问理解规则的作用

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/local.png)

# Loon 中 Rule 的类型

![image](https://raw.githubusercontent.com/chiupam/tutorial-image/master/Loon/Rule_example.png)

# 多说几句

- 规则的匹配优先次序由优先级从高到低依次排序为

  - 本地规则
  
  - 远程规则
  
  - Final,
  
- 如果在本地规则中成功匹配规则，则不会匹配远程规则下的规则，只有在本地规则和远程规则都无匹配的情况下才会执行 Final

# 参考

- [Loon 中 Rule 的类型](https://www.notion.so/Rule-878ced7042634ca994d4fc4846d60df4)
