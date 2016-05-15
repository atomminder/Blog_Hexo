title: Unbiased and Biased Estimators
date: 2016-05-13
categories: Statistics
tags: [Statistics,Math]
---

### Problem 

----------
**If a sample $ X_1,X_2 ,..., X_n $ has unknown finite variance $ \sigma^2 $, then, what is the bias between sample variance and true variance?**

----------

### Analysis

*Sample Variance Definition:*   
{% math %}
\begin{align}
S^2=\frac{1}{n}\sum_{i=1}^{n}(X_i-\overline{X})^2   \nonumber
\end{align}
{% endmath %}

----------

*Put above equation aside, consider the identity:*
{% math %}
\begin{align}
\sum_{i=1}^{n}(X_i-\mu)^2   
& {=} \sum_{i=1}^{n}((X_i-\overline{X})+(\overline{X}-\mu))^{2}     \nonumber\\
& {=} \sum_{i=1}^{n}((X_i-\overline{X})^2+2\sum_{i=1}^{n}((X_i-\overline{X})(\overline{X}-\mu))+(\overline{X}-\mu))^2   \nonumber\\
& {=} \sum_{i=1}^{n}(X_i-\overline{X})^2+\sum_{i=1}^{n}(\overline{X}-\mu)^2   \nonumber
\end{align}
{% endmath %}

----------

*So,*

{% math %} 
\begin{align}
\sum_{i=1}^{n}(X_i-\overline{X})^2{=}\sum_{i=1}^{n}(X_i-\mu)^2-\sum_{i=1}^{n}(\overline{X}-\mu)^2   \nonumber
\end{align}
{% endmath %}

*From this and sample variance definition, we can derive that:*
{% math %}
\begin{align}
{E(S^2)}  
& {=} {E}{[}\frac{1}{n}\sum_{i=1}^{n}(X_i-\mu)^2-(\overline{X}-\mu)^2{]}  \nonumber\\
& {=} \frac{1}{n}n\sigma^2-\frac{1}{n}\sigma^2  \nonumber\\
& {=} \frac{n-1}{n}\sigma^2  \nonumber
\end{align}
{% endmath %}

----------

*From above, we find that $ S^2 $ is a biased estimator for $ \sigma^2 $. *
*That is,*

{% math %}
\begin{align}
S_{biased}^{2}=S^2=\frac{1}{n}\sum_{i=1}^{n}(X_i-\overline{X})^2    \nonumber
\end{align}
{% endmath %}

*In addition, *
$$ E[\frac{n}{n-1}S^2]{=}\sigma^2 $$

*As a result,*

{% math %}
\begin{align}
S_{unbiased}^{2}{=}\frac{n}{n-1}S^2{=}\frac{1}{n-1}\sum_{i=1}^{n}(X_i-\overline{X})^2    \nonumber
\end{align}
{% endmath %}

----------

### Conclusion

{% math %}
\begin{align}
S_{biased}^{2}{=}\frac{n-1}{n}S_{unbiased}^{2}   \nonumber
\end{align}
{% endmath %}


----------

### Reference

 <i class="fa fa-rocket" aria-hidden="true"></i>  http://math.arizona.edu/~jwatkins/m-unbiased.pdf
 <i class="fa fa-rocket" aria-hidden="true"></i>   http://math.arizona.edu/~jwatkins/N_unbiased.pdf

