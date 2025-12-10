# Least Square

$$
\begin{aligned}
\boldsymbol{\beta}^*
&= \arg\min_{\boldsymbol{\beta}} \|\mathbf{y}-\mathbf{X}\boldsymbol{\beta}\|^2 \\
&= \arg\min_{\boldsymbol{\beta}}
(\mathbf{y}-\mathbf{X}\boldsymbol{\beta})^\top
(\mathbf{y}-\mathbf{X}\boldsymbol{\beta}) \\
&= \arg\min_{\boldsymbol{\beta}}
\left(
\mathbf{y}^\top\mathbf{y}
-2\boldsymbol{\beta}^\top\mathbf{X}^\top\mathbf{y}
+\boldsymbol{\beta}^\top\mathbf{X}^\top\mathbf{X}\boldsymbol{\beta}
\right) \\
\frac{\partial}{\partial \boldsymbol{\beta}}
&:
-2\mathbf{X}^\top\mathbf{y}
+2\mathbf{X}^\top\mathbf{X}\boldsymbol{\beta}=0 \\
\Rightarrow\quad
\mathbf{X}^\top\mathbf{X}\boldsymbol{\beta}
&=\mathbf{X}^\top\mathbf{y} \\
\Rightarrow\quad
\boldsymbol{\beta}
&=(\mathbf{X}^\top\mathbf{X})^{-1}\mathbf{X}^\top\mathbf{y}
\end{aligned}
$$

