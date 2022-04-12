# Bayesian Inference
Suppose that we have prior information before we look at the data. We want to incorporate that into the data somehow. We do this through [[Bayesian Inference]]. 

Suppose that we have a [[Prior Probability Distribution]] $p(\theta)$. We apply **Bayes' rule** to find the posterior (after we apply our new data) denoted $P(\theta|\mathcal{D})$. This way we can avoid working with the likelihood of the data given $\theta$ ($P(\mathcal{D}|\theta)$). 

We can do this through the equation
$$P(\theta|\mathcal{D})=\frac{P(\mathcal{D}|\theta)\times P(\theta)}{P(\mathcal{D})}=\frac{\text{Likelihood}\times\text{Prior}}{\text{Normalizing constant}}$$

Note that we typically use a [[MAP Estimate]] to find a solution