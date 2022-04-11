# P-Value
Take the $f$ from [[Significance]]. We call the p-value $p=1-f$. This tells the fraction of samples would have a more **extreme** absolute value of $T$. 


## Calculating P-Value
### 2-Sided P-value
$$p=1-\int_{-|s|}^{|s|}p_t(u;N-1)du=\int_{-\infty}^{-|s|}p_t(u;N-1)du+\int_{|s|}^{\infty}p_t(u;N-1)du$$
### 1-Sided P-value
If we want greater than $s$, 
$$p=\int_{s}^\infty p_t(u;N-1)du$$
If we want less than $s$,
$$p=\int_{-\infty}^sp_t(u;N-1)du$$