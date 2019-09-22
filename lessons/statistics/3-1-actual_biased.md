[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

```python
# Exercise 3.1 - The 'numer of children in family' paradox (similar to the 'class size' paradox)
#
# As expected, the biased PMF indicates that surveyed children (biased_pmf) respond that there
# are a higher number of children in their household (Mean: 2.4) than there actually are

# Assuming the data has been read and the resp variable has been defined...
# resp = nsfg.ReadFemResp()

pmf = thinkstats2.Pmf(resp['numkdhh'], label='numkdhh')
biased_pmf = BiasPmf(pmf, label='biased')

thinkplot.PrePlot(2)
thinkplot.Pmfs([pmf, biased_pmf])
thinkplot.Config(xlabel='Number of children', ylabel='PMF')

print('PMF mean: {}'.format(pmf.Mean())) # 1.024205155043831
print('Biased PMF mean: {}'.format(biased_pmf.Mean())) # 2.403679100664282 
```
