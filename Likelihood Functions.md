# Likelihood Functions
## Binomial
$$\mathcal{L}(\theta)={N\choose k}\theta^k(1-\theta)^{N-k}$$
This then results in the maximum at 
$$k(1-\theta)=\theta(N-k)$$
where you solve for $\theta$. 

## Geometric
$$\mathcal{L}(\theta)=(1-\theta)^{N-1}\theta$$
This then results in the maximum at
$$\hat{\theta}=\frac{1}{N}$$

## Multinomial
Say we have a multinomial distribution with $x$ probabilities we care about
$$\mathcal{L}(\theta)=\frac{n!}{\prod_{i=0}^x n_i!}\prod_{i=0}^x p_{i}^{n_i}$$
This then results in the maximum at
$$\hat{\theta}=\frac{1}{\sum_{i=0}^x n_i}(n_1, n_2,...,n_x)$$

## Poisson
$$\mathcal{L}(\theta)=\prod_{i\in\text{intervals}}\frac{\theta^{n_i}e^{-\theta}}{n_i!}$$
This then results in the maximum at 
$$\hat{\theta}=\frac{\sum_i n_i}{N}$$

## Normal
Note that for a normal distribution $\hat{\theta}$ is exactly the [[Sample Mean]]