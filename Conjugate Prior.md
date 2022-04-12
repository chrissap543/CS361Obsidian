# Conjugate Prior
Sometimes when we do $P(\theta)\times P(\mathcal{D}|\theta)$, it takes a familiar form. 

## Example 1:
Suppose that we have a coin with probability $\theta$ of coming up heads. Model the prior with a [[Beta Distribution]] with parameters $\alpha>0, \beta<0$. Flip the coin $N$ times and see $h$ heads. 
We want to find $P(\theta|N, h, \alpha, \beta)$
We then know from [[Bayesian Inference]] that
$$P(\theta|N, h, \alpha, \beta)\propto {N\choose h}\theta^h(1-\theta)^{N-h}\frac{\Gamma(\alpha+\beta)}{\Gamma(\alpha)\Gamma(\beta)}\theta^{\alpha-1}\theta^{\beta-1}$$
Note that the second half of the 'equation' is the [[Beta Distribution]]
We can also say that 
$$P(\theta|N, h, \alpha, \beta)\propto \theta^{\alpha+h-1}(1-\theta)^{\beta+N-h-1}$$
We can easily find this constant of proportionality so we have
$$P(\theta|N, h, \alpha, \beta)=\frac{\Gamma(\alpha+\beta+N)}{\Gamma(\alpha+h)\Gamma(\beta+N-h)}\theta^{\alpha+h-1}(1-\theta)^{\beta+N-h-1}$$
DON'T FORGET TO MULTIPLY BY PRIOR
after multiply, $\alpha$ is the exponent of $\theta$ plus 1 and $\beta$ is the exponent of $(1-\theta)$ plus 1
## Example 2:
Suppose that we are using a Gamma distribution as the prior for a Poisson model with the parameter $\theta$. and we are only using the first $10$ intervals of observation.
$$P(\mathcal{D}|\theta)=\frac{\theta^9e^{-10\theta}}{12}$$
$$P(\theta|\alpha, \beta)=\frac{\beta^\alpha}{\Gamma(\alpha)}\theta^{\alpha-1}e^{-\beta\theta}$$
Note that this means that we can write that
$$p(\theta|\mathcal{D}, \alpha,\beta)\propto \theta^{\alpha-1+9}e^{-(\beta+10)\theta}$$
This has the form of another gamma distribution, so we write
$$p(\theta|\mathcal{D}, \alpha, \beta)=\frac{(\beta+10)^{\alpha+9}}{\Gamma(\alpha+9)}\theta^{\alpha-1+9}e^{-(\beta+10)\theta}$$