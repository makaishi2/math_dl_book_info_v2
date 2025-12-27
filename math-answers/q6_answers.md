## Q6-1

コインを $n$ 回投げ，表が $k$ 回出たとする。  
各試行は独立で，表の出る確率は常に $p$ とする。

---

(a) 尤度関数 $L(p)$

$$
L(p)=\binom{n}{k}\,p^k(1-p)^{\,n-k}
$$

（$\binom{n}{k}$ は定数なので $L(p)\propto p^k(1-p)^{n-k}$ と書いてもよい）

(b) 対数尤度 $l(p)=\log L(p)$

$$
l(p)=\log\binom{n}{k}+k\log p+(n-k)\log(1-p)
$$

(c) 最尤推定量 $\hat p$

$$
\frac{dl}{dp}= \frac{k}{p}-\frac{n-k}{1-p}=0
$$

$$
\Longrightarrow\quad k(1-p)=p(n-k)\quad\Longrightarrow\quad \hat p=\frac{k}{n}
$$

---

## Q6-2

$X\sim N(\mu,1)$ から得られた独立標本 $x_1,\dots,x_n$ を考える。  

一般形の正規分布密度

$$
f(x)=\frac{1}{\sqrt{2\pi\sigma^2}}\exp\!\left(-\frac{(x-\mu)^2}{2\sigma^2}\right)
$$

を使う（本問では $\sigma^2=1$）

---

(a) 尤度関数 $L(\mu)$

$$
L(\mu)
=\prod_{i=1}^n f(x_i)
=(2\pi\sigma^2)^{-n/2}
\exp\!\left(-\frac{1}{2\sigma^2}\sum_{i=1}^n (x_i-\mu)^2\right)
$$

(b) 対数尤度 $l(\mu)=\log L(\mu)$

$$
l(\mu)
=-\frac{n}{2}\log(2\pi\sigma^2)
-\frac{1}{2\sigma^2}\sum_{i=1}^n (x_i-\mu)^2
$$

(c) 最尤推定量 $\hat\mu$

$$
\frac{dl}{d\mu}
=\frac{1}{\sigma^2}\sum_{i=1}^n (x_i-\mu)=0
\quad\Longrightarrow\quad
\sum_{i=1}^n x_i = n\mu
$$

$$
\hat\mu=\frac{1}{n}\sum_{i=1}^n x_i
$$
