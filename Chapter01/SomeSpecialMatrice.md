# Some Special Matrice

## Square Matrix（方阵）
1. $m=n$的matrix
2. 左上角到右下角的元素构成了一个square matrix的diagonal（对角线）
    1. 只有square matrix才有diagonal

### Upper Triangle Matrix（上三角矩阵）
Diagonal左下方所有元素都为0的矩阵

e.g.,
$$
\begin{bmatrix}
2 & 3 & 5 \\
0 & 1 & -1 \\
0 & 0 & 1
\end{bmatrix}
$$

### Lower Triangle Matrix（下三角矩阵）
Diagonal右上方所有元素都为0的矩阵

e.g.,
$$
\begin{bmatrix}
2 & 0 & 0 \\
3 & 1 & 0 \\
-1 & 1 & 1
\end{bmatrix}
$$

### Diagonal Matrix（对角矩阵）
Diagonal以外所有元素均为0的矩阵

e.g.,
$$
\begin{bmatrix}
2 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}
$$

### Identity Matrix（单位矩阵）
Diagonal上所有元素为1的diagonal matrix，记为$I$或$I_n$

e.g.,
$$
I_3=
\begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}
$$
### Zero Matrix（零矩阵）
所有元素均为0的矩阵(不一定是方阵)，记为$O$或$O_{m \times n}$

e.g.,
$$
O_{2 \times 3}=
\begin{bmatrix}
0 & 0 & 0 \\
0 & 0 & 0
\end{bmatrix}
$$

## Transpose（转置）
矩阵元素column变row，row变column的过程

如果对$m \times n$的矩阵$A$进行transpose操作可以得到一个$n \times m$的转置矩阵$A^T$

e.g.,
$$
A=
\begin{bmatrix}
6 & 9 \\
8 & 0 \\
9 & 2
\end{bmatrix}
\to  \mbox{Transpose} \to
A^T=
\begin{bmatrix}
6 & 8 & 9 \\
9 & 0 & 2
\end{bmatrix}
$$

### Properties of Transpose

假设$A,B$为$m \times n$的矩阵，$s$为标量，则有：
1. $(A^T)^T=A$
2. $(sA)^T=sA^T$
3. $(A+B)^T=A^T+B^T$
第2，3条属性就是Linear System的特征

### Symmetric Matrix（对称矩阵）
转置矩阵等于自身的矩阵，即$A=A^T$

e.g.,
$$
A=
\begin{bmatrix}
6 & 8 & 9 \\
8 & 4 & 2 \\
9 & 2 & 1
\end{bmatrix}
=A^T
$$
A是Symmetric Matrix

$$
B=
\begin{bmatrix}
6 & 8 \\
8 & 4 \\
9 & 2
\end{bmatrix}
\neq B^T
$$
B不是Symmetric Matrix
