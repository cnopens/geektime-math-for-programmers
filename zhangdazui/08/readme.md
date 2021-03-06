# 08 | 组合：如何让计算机安排世界杯的赛程？

**组合公式：**  $ C_n^m = \frac{n!}{m!(n-m)!} $

- **组合：**从 n 个元素中，任取 m (m≤n) 个元素并成一个组；
- **全组合：** 对于所有 m 取值的组合之全集合。例如对于集合{1, 2, 3}而言，全组合就是{空集, {1}, {2}, {3}, {1, 2}, {1,3} {2, 3}, {1, 2, 3}}。
  
## 思考题

Q: 假设现在需要设计一个抽奖系统。需要依次从 100 个人中，抽取三等奖 10 名，二等奖 3 名和一等奖 1 名。请列出所有可能的组合，需要注意的每人最多只能被抽中 1 次。

A:作者给出的数值太多了没法用计算机一一输出的;

从100人中选10人得3等奖，C(100, 10) = 17310309456440

再从剩下90人中选3人的3等奖，C(90, 3) = 117480

再从剩下87人中选1人得1等奖， C(87, 1) = 87

总共有大约有1.8×10^20种可能性，假设我们的计算机每1ns就能输出1个结果，全部输出来大约要5610年！假设每个结果占13个字节，把结果保存下来大约要占1995EB，远远大于世界上存储总容量！

[答案链接](https://github.com/yujiangshui/geektime-math-for-programmers/blob/master/zhangdazui/07/example.js);