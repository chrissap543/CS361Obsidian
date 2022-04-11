# Significance
The fraction of samples that would give us samples like the one we found *if* the hypothesis was true. We do this using [[Probability Distribution of Sample Mean]]. Suppose that we found our sample mean $s$. Then, we have a [[T-Distribution]] $p_t(u; N-1)$ with $N-1$ degrees of freedom. We then calculate the number of samples that will have less extreme values than $s$ as 
$$f=\frac{1}{\sqrt{2\pi}}\int_{-|s|}^{|s|}p_t(u; N-1)du$$
If $f$ is high (close to 1), we say that the data fails to support the hypothesis. 
If $f$ is low ($<.95$ typically), we say that we fail to reject the hypothesis. 

Note that if $N>30$, $p_t$ can be replaced with the density of a [[Standard Normal Distribution]]. 