# System of Linear Equations
Linear System = System of Linear Equations

## System of Linear Equations(多元一次方程组)

$$
\begin{matrix}
 {\color{Blue}{a_{11}}}{\color{Red}{x_1}}+{\color{Blue}{a_{12}}}{\color{Red}{x_2}}+\dots+{\color{Blue}{a_{1n}}}{\color{Red}{x_n}}={\color{Green}{b_1}}  \\
 {\color{Blue}{a_{21}}}{\color{Red}{x_1}}+{\color{Blue}{a_{22}}}{\color{Red}{x_2}}+\dots+{\color{Blue}{a_{2n}}}{\color{Red}{x_n}}={\color{Green}{b_2}} \\
 \vdots \\
{\color{Blue}{a_{m1}}}{\color{Red}{x_1}}+{\color{Blue}{a_{m2}}}{\color{Red}{x_2}}+\dots+{\color{Blue}{a_{mn}}}{\color{Red}{x_n}}={\color{Green}{b_m}}
\end{matrix}
$$

$$
\begin{bmatrix}x_1 \\ x_2 \\ \dots \\ x_n\end{bmatrix} \to \mbox{Linear System} \to \begin{bmatrix}b_{1} \\ b_{2} \\ \dots \\ b_{m}\end{bmatrix}
$$



1. System of Linear Equations中有$m$个equations（方程式）
2. System of Linear Equations中有$n$个variables（变量），即${\color{Red} {x_1, x_2, \dots, x_n}}$
3. 每个equation对应有$n$个coefficients（系数），即$\color{Blue}{a_{i1}, a_{i2}, \dots, a_{ij}, \dots, a_{in}}$，一共有$n \times m$个系数
4. 每个equation对应有一个常数项输出，一共有m个输出，即$\color{Green}{b_1, b_2, \dots, b_m}$
5. $n$和$m$可能是很大的数
6. 任意一个Linear System都可以写成System of Linear Equations

## Standard (Unit) Vector(标准单位向量)
1. 只有一个元素是1，其余元素都是0的向量
2. 通常用小写字母$e$加下标表示
    * 下标指1在向量中的位置
    例如：
    $e_1=\begin{bmatrix}1 \\ 0 \\ \dots \\ 0\end{bmatrix}$ $e_2=\begin{bmatrix}0 \\ 1 \\ \dots \\ 0\end{bmatrix}$ $\dots$ $e_n=\begin{bmatrix}0 \\ 0 \\ \dots \\ 1\end{bmatrix}$
3. 任意向量都可以拆解成标准单位向量的线性组合
例如：
$\mathbf{v}=\begin{bmatrix}v_1\\ v_2\end{bmatrix}=v_1 \begin{bmatrix}1\\ 0\end{bmatrix}+v_2 \begin{bmatrix}0\\ 1\end{bmatrix}=v_1 e_1+v_2 e_2$

## A linear system $\rightarrow$ A system of Linear equations

$\begin{bmatrix}1 \\ 0 \\ \dots \\ 0\end{bmatrix} \to \mbox{Linear System} \to \begin{bmatrix}a_{11} \\ a_{21} \\ \dots \\ a_{m1}\end{bmatrix}$ $\begin{bmatrix}0 \\ 1 \\ \dots \\ 0\end{bmatrix} \to \mbox{Linear System} \to \begin{bmatrix}a_{12} \\ a_{22} \\ \dots \\ a_{m2}\end{bmatrix}$ $\dots$

$\begin{bmatrix}0 \\ 0 \\ \dots \\ 1\end{bmatrix} \to \mbox{Linear System} \to \begin{bmatrix}a_{1n} \\ a_{2n} \\\dots \\ a_{mn}\end{bmatrix}$

$$\Downarrow$$

$x_1 \begin{bmatrix}1 \\ 0 \\\dots \\ 0\end{bmatrix} =\begin{bmatrix}x_1 \\ 0 \\\dots \\ 0\end{bmatrix} \to \mbox{Linear System} \to x_1 \begin{bmatrix}a_{11} \\ a_{21} \\ \dots \\ a_{m1}\end{bmatrix}=\begin{bmatrix}a_{11}x_1 \\ a_{21}x_1 \\ \dots \\ a_{m1}x_1\end{bmatrix}$

$x_2 \begin{bmatrix}0 \\ 1 \\\dots \\ 0\end{bmatrix} =\begin{bmatrix}0 \\ x_2 \\ \dots \\ 0\end{bmatrix} \to \mbox{Linear System} \to x_2 \begin{bmatrix}a_{12} \\ a_{22} \\ \dots \\ a_{m2}\end{bmatrix}=\begin{bmatrix}a_{12}x_2 \\ a_{22}x_2 \\ \dots \\ a_{m2}x_2\end{bmatrix}$

$\dots$

$x_n \begin{bmatrix}0 \\ 0 \\ \dots \\ 1\end{bmatrix} =\begin{bmatrix}0 \\ 0 \\ \dots \\ x_n\end{bmatrix} \to \mbox{Linear System} \to x_n \begin{bmatrix}a_{1n} \\ a_{2n} \\ \dots \\ a_{mn}\end{bmatrix}= \begin{bmatrix}a_{1n}x_n \\ a_{2n}x_n \\ \dots \\ a_{mn}x_n\end{bmatrix}$

$$\Downarrow$$

$\begin{bmatrix}x_1 \\ x_2 \\ \dots \\ x_n\end{bmatrix}=\begin{bmatrix}x_1 \\ 0 \\ \dots \\ 0\end{bmatrix}+\begin{bmatrix}0 \\ x_2 \\ \dots \\ 0\end{bmatrix}+ \dots+\begin{bmatrix}0 \\ 0 \\ \dots \\ x_n\end{bmatrix} \to \mbox{Linear System} \to \begin{bmatrix}a_{11}x_1+a_{12}x_2+ \dots +a_{1n}x_n \\ a_{21}x_1+a_{22}x_2 + \dots + a_{2n}x_n \\ \dots \\ a_{m1}x_1+a_{m2}x_2 + \dots + a_{mn}x_n\end{bmatrix}$
