You can also include latex style equations in markdown. Examples below demonstrate both in-line `$...$` and standalone `$$...$$` approach.
## simple example

This is a rather complex equation, which can be printed inline $\lim_{x\to 0}{\frac{e^x-1}{2x}}  \overset{\left[\frac{0}{0}\right]}{\underset{\mathrm{H}}{=}} \lim_{x\to 0}{\frac{e^x}{2}}={\frac{1}{2}}$ allowing for continous text.

In addition to what we shown in @eq:01, we can also display equations on its own:
$$z = \overbrace{
\underbrace{x}_\text{real} + i
\underbrace{y}_\text{imaginary}
}^\text{complex number}$$

as @eq:02 demonstrates.

## differences

Both equations should render properly in RStudio or in pandoc using
`pandoc math.md -s -o mathTest.html --mathjax=https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML`
, a you need to specify mathjax address.