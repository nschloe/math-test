# Test page for math in Markdown

## What works

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

#### Global newcommands

You can put `\newcommand`s in a separate block at the beginning of the page and
have all other math blocks understand the commands.

```markdown
$$
\newcommand\myexp[1]{e^{#1}}
$$

Inline: $\myexp{i}$

Display:

$$\myexp{i}$$
```

$$
\newcommand\myexp[1]{e^{#1}}
$$

Inline: $\myexp{i}$

Display:

$$\myexp{i}$$

## What doesn't work

#### Math in lists

- $E = mc^2$
- $a^2 + b^2 = c^2$

1. $V - E + F = 2$
2. $i^2 = -1$

#### Math in titles

##### This is a test title $\exp(i\pi) + 1 = 0$

#### The terminating $ can't be followed by an alphanumeric

This is rendered as math:
```markdown
An apple costs $1, a pear $.
```
An apple costs $1, a pear $.

This isn't:
```markdown
An apple costs $1, a pear $2.
```
An apple costs $1, a pear $2.

This leads to weird behavior like

```markdown
Let's try $x $y $ here.
```
Let's try $x $y $ here.


#### Copying an pasting from math blocks

#### Inline math spanned over multiple lines

$\log xy =
\log x + \log y$

#### Font is too small

ABC $ABC XYZ$ XYZ

abc $abc xyz$ xyz
