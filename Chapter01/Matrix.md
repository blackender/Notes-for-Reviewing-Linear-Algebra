# Matrix
$$
A=\begin{bmatrix}
  2 & 3 & 5\\
  3 & 1 & -1\\
  -2 & 1 & 1
\end{bmatrix}
$$

## Matrix形状

1. 如果一个matrix有m rows和n columns（即m行n列），则称该matrix是“m by n”或者“$m \times n$”
    * 表达matrix的shape（size）时先row后column
2. $\mathbf{\mathcal{M} } _{m \times n}$指所有“$m \times n$”的matrix的集合
3. vector也可看做是m行1列的matrix

eg:
1. $\begin{bmatrix}1 & 2 & 3 \\ 4 & 5 & 6\end{bmatrix} \in \mathbf{\mathcal{M} } _{2 \times 3}$
    1. 该矩阵有2 rows(2行)
    2. 该矩阵有3 columns(3列)
    3. 该矩阵是$2 \times 3$(2 by 3)
    4. 该矩阵属于$\mathbf{\mathcal{M} } _{2 \times 3}$
2. $\begin{bmatrix}1 & 4 \\ 2 & 5 \\ 3 & 6\end{bmatrix} \in \mathbf{\mathcal{M} } _{3 \times 2}$
    1. 该矩阵有3 rows(3行)
    2. 该矩阵有2 columns(2列)
    3. 该矩阵是$3 \times 2$(3 by 2)
    4. 该矩阵属于$\mathbf{\mathcal{M} } _{3 \times 2}$
3. $\begin{bmatrix}1 & 2 & 3\end{bmatrix}  \in \mathbf{\mathcal{M} } _{1 \times 3}$
    1. 该矩阵有1 rows(3行)
    2. 该矩阵有3 columns(1列)
    3. 该矩阵是$1 \times 3$(1 by 3)
    4. 该矩阵属于$\mathbf{\mathcal{M} } _{1 \times 3}$
4. $\begin{bmatrix}1 \\ 2 \\ 3\end{bmatrix}  \in \mathbf{\mathcal{M} } _{3 \times 1}$
    1. 该矩阵有3 rows(3行)
    2. 该矩阵有1 columns(1列)
    3. 该矩阵是$3 \times 1$(3 by 1)
    4. 该矩阵属于$\mathbf{\mathcal{M} } _{3 \times 1}$

## Matrix内部元素
1. 一个matrix的第i行(i-th row)，第j列(j-th column)位置的元素表达为(i, j)，即the (i, j) entry of this matrix

eg:
$A=\begin{bmatrix}2 & {\color{Red} 3} & 5 \\ 3 & 1 & -1 \\ {\color{Green} {-2}} & 1 & {\color{Blue} 1}\end{bmatrix}$
* (1, 2) entry: ${\color{Red} 3}$
* (3, 1) entry: ${\color{Green} -2}$
* (3, 3) entry: ${\color{Blue} 1}$

2. 元素索引表达为小写字母带行列下标
eg:
$A=\begin{bmatrix}a_{11} & a_{12} & \dots & a_{1n} \\ a_{21} & a_{22} & \dots & a_{2n} \\ \vdots & \vdots & \vdots & \vdots \\ a_{m1} & a_{m2} & \dots & a_{mn}\end{bmatrix}$

3. 一般可以把一个matrix中的每一列看做是一个vector，matrix也可以表达为一组列向量的序列
eg:
$A=\begin{bmatrix}\mathbf{a_1} & \mathbf{a_2} & \dots & \mathbf{a_n} \end{bmatrix}$
此时的$\mathbf{a_i}$不是vector中的第i个元素，而是matrix中的第i列

## Matrix的简单运算
如果2个matrix的shape（size）一样，则可以进行简单的加减和数乘
eg：
$A=\begin{bmatrix}1 & 4 \\ 2 & 5 \\ 3 & 6\end{bmatrix}, B=\begin{bmatrix}6 & 9 \\ 8 & 0 \\ 9 & 2\end{bmatrix} \to A+B=\begin{bmatrix}1+6 & 4+9 \\ 2+8 & 5+0 \\ 3+9 & 6+2\end{bmatrix}=\begin{bmatrix}7 & 13 \\ 10 & 5 \\ 12 & 8\end{bmatrix}$

$A=\begin{bmatrix}1 & 4 \\ 2 & 5 \\ 3 & 6\end{bmatrix}, B=\begin{bmatrix}6 & 9 \\ 8 & 0 \\ 9 & 2\end{bmatrix} \to A-B=\begin{bmatrix}1-6 & 4-9 \\ 2-8 & 5-0 \\ 3-9 & 6-2\end{bmatrix}=\begin{bmatrix}-5 & -5 \\ -6 & 5 \\ -6 & 4\end{bmatrix}$

$A=\begin{bmatrix}1 & 4 \\ 2 & 5 \\ 3 & 6\end{bmatrix} \to 3A=\begin{bmatrix}3 \times 1 & 3 \times 4 \\ 3 \times 2 & 3 \times 5 \\ 3 \times 3 & 3 \times 6\end{bmatrix}=\begin{bmatrix}3 & 12 \\ 6 & 15 \\ 9 & 18\end{bmatrix}$

## Matrix属性
如果$A$，$B$，$C$都是$m \times n$的matrix，$s$和$t$是两个scalar，则有
1. $ A+B=B+A $
2. $ (A+B)+C=A+(B+C) $
3. $ (st)A=s(tA) $
3. $ s(A+B)=sA+sB $
4. $ (s+t)A=sA+tA $

