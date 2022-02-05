# Linear System(线性系统)

## System

从input到output的复杂过程

## Linear System Conditions

1. Persevering Multiplication（均匀性/齐次性）
    * $ \triangle \to \mbox{Linear System} \to \Box \Rightarrow  k\triangle \to \mbox{Linear System} \to k\Box $
    * $ \begin{bmatrix}1\\ 2\end{bmatrix} \to \mbox{Linear System} \to \begin{bmatrix}3\\ 4\\ 5\end{bmatrix} \Rightarrow  k\begin{bmatrix}1\\ 2\end{bmatrix} \to \mbox{Linear System} \to k\begin{bmatrix}3\\ 4\\ 5\end{bmatrix} $
2. Persevering Addition（叠加性）
    * $ \begin{matrix}\triangle \to \mbox{Linear System} \to \Box\\ \diamondsuit \to \mbox{Linear System} \to \heartsuit \end{matrix}  \Rightarrow  \triangle+\diamondsuit \to \mbox{Linear System} \to \Box+\heartsuit $
    * $ \begin{matrix}\begin{bmatrix}1\\ 2\end{bmatrix} \to \mbox{Linear System} \to \begin{bmatrix}3\\ 4\\ 5\end{bmatrix}\\\begin{bmatrix}5\\ 6\end{bmatrix} \to \mbox{Linear System} \to \begin{bmatrix}7\\ 8\\ 9\end{bmatrix}\end{matrix} \Rightarrow  \begin{bmatrix}1\\ 2\end{bmatrix}+\begin{bmatrix}5\\ 6\end{bmatrix} \to \mbox{Linear System} \to \begin{bmatrix}3\\ 4\\ 5\end{bmatrix}+\begin{bmatrix}7\\ 8\\ 9\end{bmatrix} $

### Examples

#### Ex1. $ x \to \mbox{S} \to x^2 $中，S是不是linear system？
1. $ kx \to \mbox{S} \to (kx)^2=k^2x^2 \ne kx^2 $
    * 不满足Persevering Multiplication
2. $ x_1 + x_2 \to \mbox{S} \to (x_1 + x_2)^2 \ne {x_1}^2 + {x_2}^2 $
    * 不满足Persevering Addition
3. S不是linear system


#### Ex2. Transpose（转置）是不是linear system？
1. 假设有$ \begin{bmatrix}1 & 3 & 5\\ 6 & 0 & 2\end{bmatrix} \to \mbox{transpose} \to \begin{bmatrix} 1 & 6\\ 3 & 0\\ 5 & 2\end{bmatrix} $
2. $ k\begin{bmatrix}1 & 3 & 5\\ 6 & 0 & 2\end{bmatrix}=\begin{bmatrix}1k & 3k & 5k\\ 6k & 0 & 2k\end{bmatrix} \to \mbox{transpose} \to \begin{bmatrix} 1k & 6k\\ 3k & 0\\ 5k & 2k\end{bmatrix}=k\begin{bmatrix} 1 & 6\\ 3 & 0\\ 5 & 2\end{bmatrix} $
    * 满足Persevering Multiplication
3. 假设有$ \begin{bmatrix}1 & 1 & 2\\ 2 & 3 & 1\end{bmatrix} \to \mbox{transpose} \to \begin{bmatrix} 1 & 2\\ 1 & 3\\ 2 & 1\end{bmatrix} $
4. $ \begin{bmatrix}1 & 3 & 5\\ 6 & 0 & 2\end{bmatrix}+\begin{bmatrix}1 & 1 & 2\\ 2 & 3 & 1\end{bmatrix}=\begin{bmatrix}1+1 & 3+1 & 5+2\\ 6+2 & 0+3 & 2+1\end{bmatrix} \to \mbox{transpose} \to \begin{bmatrix} 1+1 & 6+2\\ 3+1 & 0+3\\ 5+2 & 2+1\end{bmatrix}=\begin{bmatrix} 1 & 6\\ 3 & 0\\ 5 & 2\end{bmatrix}+\begin{bmatrix} 1 & 2\\ 1 & 3\\ 2 & 1\end{bmatrix} $
    * 满足Persevering Addition
5. transpose是linear system


#### Ex3. Derivative（求导）是不是linear system?
1. $ f \to 求导 \to f' $
2. $ kf \to 求导 \to kf' $
    * 满足Persevering Multiplication
3. $ f+g \to 求导 \to (f+g)'=f'+g' $
    * 满足Persevering Addition
4. derivative是linear system


#### Ex4. Integrate（积分）是不是linear system?
1. $ f(x) \to \mbox{积分} \to \int_{a}^{b}f(x)dx $
2. $ kf(x) \to \mbox{积分} \to \int_{a}^{b}kf(x)dx=k\int_{a}^{b}f(x)dx $
    * 满足Persevering Multiplication
3. $ f(x)+g(x) \to \mbox{积分} \to \int_{a}^{b}[f(x)+g(x)]dx=\int_{a}^{b}f(x)dx+ \int_{a}^{b}g(x)dx $
    * 满足Persevering Addition
4. integrate是linear system
