## Math test

### What works

#### Inline math

When $a \ne 0$, there are two solutions to $(ax^2 + bx + c = 0)$ and they are
$$ x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$

Display math spanned over multiple lines:

$$
F =
G \frac{m_1m_2}{r^2}
$$

#### Math in issues and discussions

Including the _Preview_ tab, not including the title.
See https://github.com/nschloe/math-test/issues/1,
https://github.com/nschloe/math-test/discussions/2.

## What doesn't work

#### The terminating $ must be followed by whitespace

This is rendered as math:
```markdown
An apple costs $1, a pear $.
```
An apple costs $1, a pear $.



#### Using the regular dollar sign

An apple costs $1, a pear $2.

When $a \ne 0$ there.

When $a + b$ there.

When $1 2$ there.

When $1 $2 there.

When $1 $ 2 there.

When$1 $ 2 there.

When $x $2 there.

When $x $y there.

When $a + b$

When $a + b$there.

When $x $y $ there.

#### Copying an pasting from math blocks

#### Math in lists

- $E = mc^2$
- $a^2 + b^2 = c^2$

1. $V - E + F = 2$
2. $i^2 = -1$

#### Inline math spanned over multiple lines

$\log xy =
\log x + \log y$

#### Math in titles $\exp(i\pi) + 1 = 0$

#### Font is too small

A $A$ x $x$
