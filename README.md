# Test page for math in Markdown

#### Inline and display math

When $a \ne 0$, there are two solutions to $(ax^2 + bx + c = 0)$ and they are

$$
x = {-b \pm \sqrt{b^2-4ac} \over 2a}.
$$

Inline math spanned over multiple lines: $\log xy =
\log x + \log y$

Display math spanned over multiple lines:

$$
F =
G \frac{m_1m_2}{r^2}
$$

#### Math in lists

- $E = mc^2$
- $a^2 + b^2 = c^2$

1. $V - E + F = 2$
2. $i^2 = -1$

#### Math in titles $\exp(i\pi) + 1 = 0$

#### Math in tables

The Butcher tableau for this ERK method is

| $0$   |       |       |       |       |
| ----- | :---: | ----: | ----: | ----: |
| $1/2$ | $1/2$ |       |       |       |
| $1/2$ |  $0$  | $1/2$ |       |       |
| $1$   |  $0$  |   $0$ |   $1$ |       |
|       | $1/6$ | $1/3$ | $1/3$ | $1/6$ |

#### Global newcommands

Newcommand block (no output):

$$
\newcommand\myexp[1]{e^{#1}}
$$

Inline math that uses the newcommand: $\myexp{i}$

Display that uses the newcommand:

$$
\myexp{i}
$$

#### $-confusion

- ```markdown
  An apple costs $1, a pear $.
  ```

  An apple costs $1, a pear $2.

- ```markdown
  An apple costs 1$, a pear 2$.
  ```

  An apple costs 1$, a pear 2$.

- ```markdown
  Let's try $x $y $ here.
  ```
  Let's try $x $y $ here.

#### Font size comparison

ABC $ABC XYZ$ XYZ

abc $abc xyz$ xyz

#### Cauchy's Theorem

Let $U$ be an open subset of the complex plane $\mathbb{C}$, and suppose the
closed disk $D$ defined as

$$
D = \{z:|z-z_{0}|\leq r\}
$$

is completely contained in $U$. Let $f: U\to\mathbb{C}$ be a holomorphic function,
and let $\gamma$ be the circle, oriented counterclockwise, forming the boundary of
$D$. Then for every $a$ in the interior of $D$,

$$
f(a) = \frac{1}{2\pi i} \oint_{\gamma}\frac{f(z)}{z-a}\,dz.
$$
