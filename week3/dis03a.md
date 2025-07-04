# CS 70 2024年春季 离散数学与概率论 Seshia, Sinclair

### DIS 3A

## 1 派对技巧


你正在参加一个派对，庆祝自己完成了CS 70期中考试。通过快速算出下列各数的最后一位数字，来展示你的模运算技巧，给朋友们留下深刻印象：

(a) 求 113142 的最后一位数字。

(b) 求 99999 的最后一位数字。

(c) 求 3641 的最后一位数字。

## 2 模运算杂烩


证明或反驳以下陈述：

(a) 存在某个整数 $x\in\mathbb{Z}$，使得 $x\equiv3$ (mod 16) 且 $x\equiv4$ (mod 6)。

(b) 若 $2x\equiv4$ (mod 12)，则 $x\equiv2$ (mod 12)。

(c) 若 $2x\equiv4$ (mod 12)，则 $x\equiv2$ (mod 6)。


## 3 模逆元


回顾讲座中关于逆元的定义：设 $a,m\in\mathbb{Z}$ 且 $m>0$，如果 $x\in\mathbb{Z}$ 满足 $ax\equiv1$ (mod m)，那么我们称 x 是 a 模 m 的一个逆元。

现在，我们将研究逆元的存在性和唯一性。

(a) 3 是 5 模 10 的逆元吗？

(b) 3 是 5 模 14 的逆元吗？

(c) 对于所有 $n\in\mathbb{N}$，$3+14n$ 是 5 模 14 的逆元吗？

(d) 4 模 8 有逆元吗？

(e) 假设 $x,x^{\prime}\in\mathbb{Z}$ 都是 a 模 m 的逆元。是否可能 $x\not\equiv x^{\prime}$ (mod m)？

## 4 斐波那契最大公约数

斐波那契数列由 $F_{n}=F_{n-1}+F_{n-2}$ 给出，其中 $F_{0}=0$ 且 $F_{1}=1$。证明对于所有 $n\ge1$，$gcd(F_{n},F_{n-1})=1$。