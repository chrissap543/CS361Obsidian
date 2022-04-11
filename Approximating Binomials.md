# Approximating Binomials
For large $N$, the binomial probability distribution function becomes the [[Standard Normal Distribution]] where we have that 
$$x=\frac{h-Np}{\sqrt{Npq}}$$
We can use this to calculate the probability of $x\in[a, b]$ as
$$\int_a^b\left(\frac{1}{\sqrt{2\pi}}\right)e^{\frac{-u^2}{2}}du$$
where $a$ and $b$ are like number of heads that a coin will have after $N$ flips. 