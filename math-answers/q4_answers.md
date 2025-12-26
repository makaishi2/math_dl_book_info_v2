
## Q4-1

2 変数関数  

$$
L(u,v)=\frac12\bigl((u-p)^2+(v-q)^2\bigr)+\lambda(u^2+v^2)
$$

について考える（$p,q,\lambda$ は定数）。

 (a) $u$ に関する偏微分を計算せよ

---

$$
\frac{\partial L}{\partial u}
=(u-p)+2\lambda u
=(1+2\lambda)u-p
$$

(b) $v$ に関する偏微分を計算せよ

---

$$
\frac{\partial L}{\partial v}
=(v-q)+2\lambda v
=(1+2\lambda)v-q
$$

(c) $p=2,\ q=-1,\ \lambda=1$， $(u,v)=(0,0)$のとき、偏微分の計算結果を求めよ

---

$$
\frac{\partial L}{\partial u}=3u-p,\qquad
\frac{\partial L}{\partial v}=3v-q
$$

よって，

$$
\left.\frac{\partial L}{\partial u}\right|_{(0,0)}=-2,
\qquad
\left.\frac{\partial L}{\partial v}\right|_{(0,0)}=1
$$

したがって，

$$
\nabla L(0,0)=(-2,\,1)
$$

---

## Q4-2

合成関数 $L(x_1,x_2)=L(u(x_1,x_2),v(x_1,x_2))$ を
$x_1$ で偏微分せよ。

---

$$
L(u,v)=\frac12\bigl((u-p)^2+(v-q)^2\bigr)+\lambda(u^2+v^2),
$$

$$
u(x_1,x_2)=w_{11}x_1+w_{12}x_2,\qquad
v(x_1,x_2)=w_{21}x_1+w_{22}x_2
$$

（$p,q,\lambda,w_{11},w_{12},w_{21},w_{22}$ は定数）

1. まず $\partial L/\partial u,\ \partial L/\partial v$

$$
\frac{\partial L}{\partial u}=(1+2\lambda)u-p,
\qquad
\frac{\partial L}{\partial v}=(1+2\lambda)v-q
$$

2. 連鎖律（チェインルール）

$$
\frac{\partial L}{\partial x_1}
=\frac{\partial L}{\partial u}\frac{\partial u}{\partial x_1}
+\frac{\partial L}{\partial v}\frac{\partial v}{\partial x_1}
$$

$$
\frac{\partial u}{\partial x_1}=w_{11}, \qquad
\frac{\partial v}{\partial x_1}=w_{21}
$$

したがって

$$
\frac{\partial L}{\partial x_1}
=\left((1+2\lambda)u-p\right)w_{11}
+\left((1+2\lambda)v-q\right)w_{21}
$$

3. $u,v$ を $x_1,x_2$ で書き換える

$$
u=w_{11}x_1+w_{12}x_2,\qquad
v=w_{21}x_1+w_{22}x_2
$$

代入して

$$
\frac{\partial L}{\partial x_1}
=
\Bigl((1+2\lambda)(w_{11}x_1+w_{12}x_2)-p\Bigr)w_{11}
+
\Bigl((1+2\lambda)(w_{21}x_1+w_{22}x_2)-q\Bigr)w_{21}
$$

これが求める結果である。
