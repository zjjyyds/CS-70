# CS 70 离散数学与概率论
春季 2024 Seshia, Sinclair
DIS 1A

## 1 自然归纳法应用于不等式
**笔记 3** 证明：如果 $n \in \mathbb{N}$ 且 $x > 0$，则 $(1 + x)^n \geq 1 + n x$。

## 2 加强证明

**笔记 3** 假设序列 $a_1, a_2, \ldots$ 由 $a_1 = 1$ 以及对于 $n \geq 1$ 的 $a_{n+1} = 3 a_n^2$ 定义。我们想证明：

$$
a_n \leq 3^{\left(2^n\right)}
$$

对于每个正整数 $n$。
(a) 假设我们想使用归纳法证明这个陈述。我们的归纳假设可以简单地是 $a_n \leq 3^{\left(2^n\right)}$ 吗？尝试用这个假设进行归纳证明，说明为什么这行不通。
(b) 尝试改为用归纳法证明陈述 $a_n \leq 3^{\left(2^n - 1\right)}$。
(c) 为什么 (b) 部分的假设暗示了整体的结论？

CS 70, 春季 2024, DIS 1A
1

---

## 3 二进制数
**笔记 3** 证明每个正整数 $n$ 都可以用二进制表示。换句话说，证明对于任意正整数 $n$，我们可以写成：

$$
n = c_k \cdot 2^k + c_{k-1} \cdot 2^{k-1} + \cdots + c_1 \cdot 2^1 + c_0 \cdot 2^0,
$$

其中存在某个 $k \in \mathbb{N}$ 且对于所有 $i \leq k$，$c_i \in \{0, 1\}$。

## 4 斐波那契数在家练习
**笔记 3** 回想一下，斐波那契数递归定义为：

$$
F_1 = 1, F_2 = 1 \text{, 且 } F_n = F_{n-2} + F_{n-1}。
$$

证明每个第三个斐波那契数都是偶数。例如，$F_3 = 2$ 是偶数，$F_6 = 8$ 是偶数。

CS 70, 春季 2024, DIS 1A
2