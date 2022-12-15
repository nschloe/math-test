# Test page for math in Markdown

#### Bugs

##### Two brackets

```markdown
$[a+b](c+d)$
```

$[a+b](c+d)$

##### Backslashes in `$`-math https://github.com/community/community/discussions/16993

```markdown
$\{a\}$
```

$\{a\}$

##### Oversized sqrt symbol around fractions https://github.com/community/community/discussions/39251

```math
\sqrt{\frac{1}{2}}
```

##### Sum in fraction https://github.com/community/community/discussions/39432

```math
\frac{\sum_{i=1}^n}{2}
```

##### Dollar in `\text` https://github.com/community/community/discussions/39655

```math
a
```

- ```math
  \text{$b$}
  ```

##### Issues with underscores

- https://github.com/community/community/discussions/30747

  ```markdown
  ${a}_b c_{d}$
  ```

  ${a}_b c_{d}$

- https://github.com/community/community/discussions/41087

  ```markdown
  $[x]_y a_{b}$
  ```

  $[x]_y a_{b}$

#### Inline and display math

When $a \ne 0$, there are two solutions to $(ax^2 + bx + c = 0)$ and they are

```math
x = {-b \pm \sqrt{b^2-4ac} \over 2a}.
```

Inline math spanned over multiple lines: $\log xy =
\log x + \log y$

Display math spanned over multiple lines:

```math
F =
G \frac{m_1m_2}{r^2}
```

##### Cauchy's Theorem

Let $U$ be an open subset of the complex plane $\mathbb{C}$, and suppose the
closed disk $D$ defined as

```math
D = \{z:|z-z_{0}|\leq r\}
```

is completely contained in $U$. Let $f: U\to\mathbb{C}$ be a holomorphic function,
and let $\gamma$ be the circle, oriented counterclockwise, forming the boundary of
$D$. Then for every $a$ in the interior of $D$,

```math
f(a) = \frac{1}{2\pi i} \oint_{\gamma}\frac{f(z)}{z-a}\,dz.
```

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

```math
\newcommand\myexp[1]{e^{#1}}
```

Inline math that uses the newcommand: $\myexp{i}$

Display that uses the newcommand:

```math
\myexp{i}
```

#### $-confusion?

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

- ```markdown
  $x = \text{my $y$}$
  ```

  $x = \text{my $y$}$

- ```markdown
  $x =\$$
  ```
  $x =\$$

#### Font size comparison

ABC $ABC XYZ$ XYZ

abc $abc xyz$ xyz

#### Other LaTeX commands

- ```markdown
  \{n\in\mathbb{N}:\: n\,\text{even}\}
  ```

  ```math
  \{n\in\mathbb{N}:\: n\,\text{even}\}
  ```

- ```markdown
  a <b > c
  ```
  ```math
  a <b > c
  ```
