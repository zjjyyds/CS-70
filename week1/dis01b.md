# CS 70 离散数学与概率论
春季 2024
Seshia, Sinclair
DIS 1B

## 1 稳定匹配
**笔记 4**
考虑工作岗位集合 $J = \{1, 2, 3\}$ 和求职者集合 $C = \{A, B, C\}$，其偏好如下。

<table>
  <tr>
    <th style="text-align: center; vertical-align: middle;">工作岗位(Jobs)</th>
    <th colspan="3" style="text-align: center; vertical-align: middle;">求职者(Candidates)</th>
  </tr>
  <tr>
    <td style="text-align: center; vertical-align: middle;">1</td>
    <td style="text-align: center; vertical-align: middle;">A</td>
    <td style="text-align: center; vertical-align: middle;">B</td>
    <td style="text-align: center; vertical-align: middle;">C</td>
  </tr>
  <tr>
    <td style="text-align: center; vertical-align: middle;">2</td>
    <td style="text-align: center; vertical-align: middle;">B</td>
    <td style="text-align: center; vertical-align: middle;">A</td>
    <td style="text-align: center; vertical-align: middle;">C</td>
  </tr>
  <tr>
    <td style="text-align: center; vertical-align: middle;">3</td>
    <td style="text-align: center; vertical-align: middle;">A</td>
    <td style="text-align: center; vertical-align: middle;">B</td>
    <td style="text-align: center; vertical-align: middle;">C</td>
  </tr>
</table>

<table>
  <tr>
    <th style="text-align: center; vertical-align: middle;">求职者(Candidates)</th>
    <th colspan="3" style="text-align: center; vertical-align: middle;">工作岗位(Jobs)</th>
  </tr>
  <tr>
    <td style="text-align: center; vertical-align: middle;">A</td>
    <td style="text-align: center; vertical-align: middle;">2</td>
    <td style="text-align: center; vertical-align: middle;">1</td>
    <td style="text-align: center; vertical-align: middle;">3</td>
  </tr>
  <tr>
    <td style="text-align: center; vertical-align: middle;">B</td>
    <td style="text-align: center; vertical-align: middle;">1</td>
    <td style="text-align: center; vertical-align: middle;">3</td>
    <td style="text-align: center; vertical-align: middle;">2</td>
  </tr>
  <tr>
    <td style="text-align: center; vertical-align: middle;">C</td>
    <td style="text-align: center; vertical-align: middle;">1</td>
    <td style="text-align: center; vertical-align: middle;">2</td>
    <td style="text-align: center; vertical-align: middle;">3</td>
  </tr>
</table>

运行传统的提出-拒绝算法在这个例子上。需要多少天？结果配对是什么？（展示你的工作过程。）


---

## 2 提出-拒绝证明
**笔记 4**
证明以下关于传统提出-拒绝算法的陈述。
(a) 在算法的任何执行中，如果一名求职者在第 $i$ 天收到一个建议，那么在此后直到算法终止的每一天她都会收到一些建议。

(b) 在算法的任何执行中，如果一名求职者在第 $i$ 天没有收到建议，那么她在前一天 $j$（$1 \leq j < i$）也没有收到建议。

(c) 在算法的任何执行中，至少有一名求职者只收到一个建议。（提示：使用上面的部分！）


---

## 3 当裁判
**笔记 4**
我们将稳定匹配实例定义为工作岗位和求职者及其偏好列表的集合。对于以下每个陈述，指出该陈述是真还是假，并用 2-3 行的简短解释证明您的答案：
(a) 对于 $n > 1$ 的 $n$ 个工作岗位和 $n$ 个求职者，存在一个稳定匹配实例，使得在工作岗位提议的稳定匹配算法中，每个工作岗位最终都与它最不喜欢的求职者配对。

(b) 在一个稳定匹配实例中，如果工作岗位 $J$ 和求职者 $C$ 各自在对方偏好列表的顶部，那么 $J$ 必须在每个稳定配对中与 $C$ 配对。

(c) 在至少有两个工作岗位和两个求职者的稳定匹配实例中，如果工作岗位 $J$ 和求职者 $C$ 各自在对方偏好列表的底部，那么 $J$ 不能在任何稳定配对中与 $C$ 配对。

(d) 对于每个 $n > 1$，存在一个 $n$ 个工作岗位和 $n$ 个求职者的稳定匹配实例，其中存在一个不稳定的配对，所有未匹配的工作岗位-求职者对都是流氓配对或配对。



---

## 4 稳定匹配 III
**笔记 4**
(a) 真或假？

(i) 如果一名求职者在某一天意外拒绝了她更喜欢的某项工作，那么算法仍然总是以匹配结束。

(ii) 提出-拒绝算法从不产生求职者最优的匹配。

(iii) 如果同一项工作在每个求职者的偏好列表中排在最后，那么该工作必须最终与它最不喜欢的求职者配对。

(b) 正如您在讲座中看到的，工作岗位提议的提出-拒绝算法会产生雇主最优的稳定匹配。现在让我们看看求职者是否有办法改善他们的地位。假设只有一名求职者有权力随意拒绝一个求职建议，无论她当前是否持有某项工作（如果有）。构造一个示例，说明以下内容：对于任意 $n \geq 2$，存在一个稳定匹配实例，使用这种权力对每个求职者都有帮助，即每个求职者都得到了比工作岗位提议的提出-拒绝算法下更好的工作。

