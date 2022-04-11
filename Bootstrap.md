# Bootstrap
Our previous formulas for [[Standard Error]] work very well for [[Sample Mean]]. But if we wanted to do work on medians or other interesting statistics? It is difficult mathematically.
We use a **bootstrap** to give a very good estimate of the [[Standard Error]]. Denote a statistic $S(x)$ as a function of the dataset of $N$ items. We compute $r$ **bootstrap replications** by sampling the dataset uniformly **with replacement**. This [[Continuous Uniform Distribution]] is known as the empirical distribution and has probability $\frac{1}{N}$ at each item within the sample and $0$ everywhere else. Draw [[IID Samples]] from this distribution. Then compute the mean of these and the [[Standard Error]] where $N=r$. 