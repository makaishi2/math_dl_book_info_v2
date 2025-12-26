## Q5-1

次のように定義される関数の微分を求めよ。

$$
\tanh(x)=\frac{e^x-e^{-x}}{e^x+e^{-x}}
$$

---

分子を $f(x)=e^x-e^{-x}$，分母を $g(x)=e^x+e^{-x}$ とおく。

$$
f'(x)=e^x+e^{-x},\qquad
g'(x)=e^x-e^{-x}
$$

商の微分より，

$$
(\tanh x)'=\frac{f'(x)g(x)-f(x)g'(x)}{g(x)^2}
$$

$$
(\tanh x)'
=\frac{(e^x+e^{-x})^2-(e^x-e^{-x})^2}{(e^x+e^{-x})^2}
=\frac{4}{(e^x+e^{-x})^2}
$$

さらに，

$$
1-\tanh^2 x=\frac{4}{(e^x+e^{-x})^2}
$$

したがって，

$$
(\tanh x)' = 1-\tanh^2 x
$$

---

## Q5-2

次のように定義される関数の微分を求めよ（$t$ は定数）

$$
e(p)=t\log(p)+(1-t)\log(1-p)
$$

---

$$
\frac{d}{dp}\bigl(t\log p\bigr)=\frac{t}{p},
\qquad
\frac{d}{dp}\bigl((1-t)\log(1-p)\bigr)
= -\frac{1-t}{1-p}
$$

したがって，

$$
e'(p)=\frac{t}{p}-\frac{1-t}{1-p}
$$

整理すると，

$$
e'(p)=\frac{t-p}{p(1-p)}
$$

