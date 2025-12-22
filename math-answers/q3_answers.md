
## Q3-1
次のベクトルの絶対値を求めよ。

$$
\mathbf{a}=(15,\,36)
$$

---

### 解答
$$
|\mathbf{a}|=\sqrt{15^2+36^2}
=\sqrt{225+1296}
=\sqrt{1521}
=39
$$

---

## Q3-2
次の 2 つのベクトルの距離を求めよ。

$$
\mathbf{b}=(9,\,2,\,4),\quad
\mathbf{c}=(6,\,-3,\,8)
$$

---

### 解答
距離は差ベクトルの絶対値である。

$$
\mathbf{b}-\mathbf{c}
=(9-6,\;2-(-3),\;4-8)
=(3,\,5,\,-4)
$$

$$
\text{距離}
=\sqrt{3^2+5^2+(-4)^2}
=\sqrt{9+25+16}
=\sqrt{50}
=5\sqrt{2}
$$

---

## Q3-3
次の 2 つのベクトルのなす角を求めよ。

$$
\mathbf{u}=(4,\,1,\,1),\quad
\mathbf{v}=(1,\,1,\,4)
$$

---

### 解答
まず内積を計算する。

$$
\mathbf{u}\cdot\mathbf{v}
=4\cdot1+1\cdot1+1\cdot4
=4+1+4
=9
$$

次に、それぞれの絶対値を求める。

$$
|\mathbf{u}|=\sqrt{4^2+1^2+1^2}
=\sqrt{16+1+1}
=\sqrt{18}
$$

$$
|\mathbf{v}|=\sqrt{1^2+1^2+4^2}
=\sqrt{1+1+16}
=\sqrt{18}
$$

なす角を $$\theta$$ とすると、

$$
\cos\theta
=\frac{\mathbf{u}\cdot\mathbf{v}}{|\mathbf{u}||\mathbf{v}|}
=\frac{9}{\sqrt{18}\sqrt{18}}
=\frac{9}{18}
=\frac{1}{2}
$$

よって、

$$
\theta=60^\circ
$$

---

## Q3-4
次の 3 つのベクトル間の **コサイン類似度** を求め、
「最も近い 2 つのベクトル」の組を見つけよ。

$$
\mathbf{a}=(-3,\,-3,\,-3,\,-3)
$$

$$
\mathbf{b}=(-3,\,-2,\,-2,\,1)
$$

$$
\mathbf{c}=(-4,\,1,\,4,\,-2)
$$

---

### 解答
コサイン類似度は

$$
\cos(\mathbf{x},\mathbf{y})
=\frac{\mathbf{x}\cdot\mathbf{y}}{|\mathbf{x}||\mathbf{y}|}
$$

である。

---

### 1) ノルム
$$
|\mathbf{a}|=\sqrt{(-3)^2+(-3)^2+(-3)^2+(-3)^2}
=\sqrt{36}
=6
$$

$$
|\mathbf{b}|=\sqrt{(-3)^2+(-2)^2+(-2)^2+1^2}
=\sqrt{9+4+4+1}
=\sqrt{18}
$$

$$
|\mathbf{c}|=\sqrt{(-4)^2+1^2+4^2+(-2)^2}
=\sqrt{16+1+16+4}
=\sqrt{37}
$$

---

### 2) 内積とコサイン類似度

#### (a, b)
$$
\mathbf{a}\cdot\mathbf{b}
=(-3)(-3)+(-3)(-2)+(-3)(-2)+(-3)(1)
=9+6+6-3
=18
$$

$$
\cos(\mathbf{a},\mathbf{b})
=\frac{18}{6\sqrt{18}}
=\frac{3}{\sqrt{18}}
=\frac{1}{\sqrt{2}}
$$

#### (a, c)
$$
\mathbf{a}\cdot\mathbf{c}
=(-3)(-4)+(-3)(1)+(-3)(4)+(-3)(-2)
=12-3-12+6
=3
$$

$$
\cos(\mathbf{a},\mathbf{c})
=\frac{3}{6\sqrt{37}}
=\frac{1}{2\sqrt{37}}
$$

#### (b, c)
$$
\mathbf{b}\cdot\mathbf{c}
=(-3)(-4)+(-2)(1)+(-2)(4)+1(-2)
=12-2-8-2
=0
$$

$$
\cos(\mathbf{b},\mathbf{c})=0
$$

---

### 3) 最も近い組
$$
\cos(\mathbf{a},\mathbf{b})=\frac{1}{\sqrt{2}}
,\quad
\cos(\mathbf{a},\mathbf{c})=\frac{1}{2\sqrt{37}}
,\quad
\cos(\mathbf{b},\mathbf{c})=0
$$

よってコサイン類似度が最大なのは $$\mathbf{a}$$ と $$\mathbf{b}$$ である。

$$
\boxed{\text{最も近い 2 つのベクトルは }\mathbf{a}\text{ と }\mathbf{b}}
$$

## Q3-5
次の行列とベクトルのかけ算を計算せよ。

$$
\begin{pmatrix}
2 & -1 \\
4 & 3 \\
-5 & 6
\end{pmatrix}
\begin{pmatrix}
3 \\
2
\end{pmatrix}
$$

---

### 解答
行列とベクトルの積は、**各行とベクトルの内積**で計算する。

#### 第1成分
$$
2\cdot 3 + (-1)\cdot 2
=6-2
=4
$$

#### 第2成分
$$
4\cdot 3 + 3\cdot 2
=12+6
=18
$$

#### 第3成分
$$
(-5)\cdot 3 + 6\cdot 2
=-15+12
=-3
$$

### 結果

$$
\begin{pmatrix}
2 & -1 \\
4 & 3 \\
-5 & 6
\end{pmatrix}
\begin{pmatrix}
3 \\
2
\end{pmatrix}
=
\begin{pmatrix}
4 \\
18 \\
-3
\end{pmatrix}
$$

