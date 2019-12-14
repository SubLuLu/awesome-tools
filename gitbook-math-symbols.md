# gitbook中使用数学公式

使用gitbook编写markdown时，如果需要使用数学公式，可以通过插件方式安装`katex`来进行支持，在book.json中添加如下配置即可:

```json
"plugins": [
  "katex"
]
```

### 符号

| 符号 | 输入    |
| ---- | ------- |
| ∃    | \exists |
| ∀    | \forall |
| 空格 | \quad   |
| ∞    | \infty  |

大多数常见的数学符号可以在[Detexify](http://detexify.kirelabs.org/classify.html)上通过手写识别

### 希腊字母

| 字母 | 输入        |
| ---- | ----------- |
| α    | \alpha      |
| β    | \beta       |
| γ    | \gamma      |
| δ    | \delta      |
| ϵ    | \epsilon    |
| ε    | \varepsilon |
| ζ    | \zeta       |
| η    | \eta        |
| θ    | \theta      |
| ϑ    | \vartheta   |
| ι    | \iota       |
| κ    | \kappa      |
| λ    | \lambda     |
| μ    | \mu         |
| ν    | \nu         |
| ξ    | \xi         |
| o    | o           |
| π    | \pi         |
| ϖ    | \varpi      |
| ρ    | \rho        |
| ϱ    | \varrho     |
| σ    | \sigma      |
| ς    | \varsigma   |
| τ    | \tau        |
| υ    | \upsilon    |
| ϕ    | \phi        |
| φ    | \varphi     |
| χ    | \chi        |
| ψ    | \psi        |
| ω    | \omega      |
| Γ    | \Gamma      |
| Λ    | \Lambda     |
| Σ    | \Sigma      |
| Ψ    | \Psi        |
| Δ    | \Delta      |
| Ξ    | \Xi         |
| Υ    | \Upsilon    |
| Ω    | \Omega      |
| Θ    | \Theta      |
| Π    | \Pi         |
| Φ    | \Phi        |

### 二元关系符

| 符号 | 输入        | 符号 | 输入        | 符号 | 输入    |
| ---- | ----------- | ---- | ----------- | ---- | ------- |
| <    | <           | >    | >           | =    | =       |
| ≤    | \leq或\le   | ≥    | \geq或\ge   | ≡    | \equiv  |
| ⩽    | \leqslant   | ⩾    | \geqslant   |      |         |
| ≪    | \ll         | ≫    | \gg         | ≐    | \doteq  |
| ≺    | \prec       | ≻    | \succ       | ∼    | \sim    |
| ⪯    | \preceq     | ⪰    | \succeq     | ≃    | \simeq  |
| ⊂    | \subset     | ⊃    | \supset     | ≈    | \approx |
| ⊆    | \subseteq   | ⊇    | \supseteq   | ≅    | \cong   |
| ⊏    | \sqsubset   | ⊐    | \sqsupset   | ⋈    | \Join   |
| ⊑    | \sqsubseteq | ⊒    | \sqsupseteq | ⋈    | \bowtie |
| ∈    | \in         | ∋    | \ni或\owns  | ∝    | \propto |
| ⊢    | \vdash      | ⊣    | \dashv      | ⊨    | \models |
| ∣    | \mid        | ∥    | \parallel   | ⊥    | \perp   |
| ⌣    | \smile      | ⌢    | \frown      | ≍    | \asymp  |
|   :   |       :      |    ∉  |    \notin         |  ≠    |     \neq    |

### 二元运算符

| 符号 | 输入           | 符号 | 输入             | 符号 | 输入           |
| ---- | -------------- | ---- | ---------------- | ---- | -------------- |
| +    | +              | −    | -                |      |                |
| ±    | \pm            | ∓    | \mp              | ◃    | \triangleleft  |
| ⋅    | \cdot          | ÷    | \div             | ▹    | \triangleright |
| ×    | \times         | ∖    | \setminus        | ⋆    | \star          |
| ∪    | \cup           | ∩    | \cap             | ∗    | \ast           |
| ⊔    | \sqcup         | ⊓    | \sqcap           | ∘    | \circ          |
| ∨    | \vee或\lor     | ∧    | \wedge或\land    | ∙    | \bullet        |
| ⊕    | \oplus         | ⊖    | \ominus          | ⋄    | \diamond       |
| ⊙    | \odot          | ⊘    | \oslash          | ⊎    | \uplus         |
| ⊗    | \otimes        | ◯    | \bigcirc         | ⨿    | \amalg         |
| △    | \bigtriangleup | ▽    | \bigtriangledown | †    | \dagger        |
| ⊲    | \lhd           | ⊳    | \rhd             | ‡    | \ddagger       |
| ⊴    | \unlhd         | ⊵    | \unrhd           | ≀    | \wr            |

### 格式

| 效果         | 输入      |
| ------------ | --------- |
| 上标         | ^         |
| 下标         | _         |
| 加粗         | \textbf{} |
| 倾斜         | \emph{}   |
| 分数         | \frac{}{} |
| 根式         | \sqrt[]{} |
| 省略号       | \ldots    |
| 改变左边高度  | \left     |
| 改变右边高度  | \right    |

### 矩阵和行列式

```
A = \left[ \begin{matrix}

   a & b  \\

   c & d  \\

\end{matrix} \right]
```

$$A = \left[ \begin{matrix}

   a & b  \\

   c & d  \\

\end{matrix} \right] $$

```
\chi (\lambda)=\left| \begin{matrix}

   \lambda - a & -b  \\

   -c & \lambda - d  \\

\end{matrix} \right|
```

$$\chi (\lambda)=\left| \begin{matrix}

   \lambda - a & -b  \\

   -c & \lambda - d  \\

\end{matrix} \right| $$

### 求和与连乘

```
\sum_{k=1}^n k^2 = \frac{1}{2} n (n+1)
```

$$\sum_{k=1}^n k^2 = \frac{1}{2} n (n+1)$$

```
\prod_{k=1}^n k = n!
```

$$\prod_{k=1}^n k = n!$$

### 导数

```
{f}'(x) = x^2 + x
```

$${f}'(x) = x^2 + x$$

### 极限

```
\lim_{x \to 0} \frac{3x^2 +7x^3}{x^2 +5x^4} = 3
```

$$\lim_{x \to 0} \frac{3x^2 +7x^3}{x^2 +5x^4} = 3$$

### 积分

在多重积分内 dx 和 dy 之间 使用一个斜杠加一个逗号 \, 来增大稍许间距。同样，在两个积分号之间使用一个斜杠加一个感叹号 \! 来减小稍许间距。

```
\int_a^b f(x)\,dx
```

$$\int_a^b f(x)\,dx$$

```
\int_{x^2 + y^2 \leq R^2} f(x,y)\,dx\,dy = \int_{\theta=0}^{2\pi} \int_{r=0}^R f(r\cos\theta,r\sin\theta) r\,dr\,d\theta
```

$$\int_{x^2 + y^2 \leq R^2} f(x,y)\,dx\,dy = \int_{\theta=0}^{2\pi} \int_{r=0}^R f(r\cos\theta,r\sin\theta) r\,dr\,d\theta$$

```
\int \!\!\! \int_D f(x,y)\,dx\,dy \int \int_D f(x,y)\,dx\,dy
```

$$\int \!\!\! \int_D f(x,y)\,dx\,dy \int \int_D f(x,y)\,dx\,dy$$
