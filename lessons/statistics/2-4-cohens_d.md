[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

```python
# Exercise 2.4 - Are first babies lighter or heavier than others?

# Note: I used the existing Think Stats Cohen effect size function/abstraction
# (i.e. `CohenEffectSize(...`)... Note: The code below assumes this function and all
# the required dependencies/imports are available and that the data is available
# in `firsts` and `others`

firsts_total_weight = firsts.totalwgt_lb
others_total_weight = others.totalwgt_lb

# The difference in means is -0.088672927072602 standard deviations
#
# Since firsts_total_weight is the experimental group and others_total_weight is the
# control group, a negative effect size indicates that the effect decreases the mean
CohenEffectSize(firsts_total_weight, others_total_weight)
```
