[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

```python
import scipy.stats

mu = 178 # Mean
sigma = 7.7 # Standard deviation

dist = scipy.stats.norm(loc=mu, scale=sigma)

blue_man_shortest = dist.cdf(177.8) # 5'10" in centimeters
high = dist.cdf(185.4) # 6'1" in centimeters

print('Percentage of US males that could be a Blue Man: {}'.format((high - low) * 11)) # 34.20%
```
