[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

>> The code for generating a sample of 1000 data points and for plotting its PMF is as follows
```python
sample = np.random.random(1000)
sample_pmf = thinkstats2.Pmf(sample)
thinkplot.Hist(sample_pmf)
thinkplot.Config(xlabel='value', ylabel='PMF')
```

>> The resultant PMF histogram comes up empty:

![PMF of continuous random values form 0 to 1] (http://i.imgur.com/2AYkBTs.png)

>> This may be due to the fact that the variable is continuous and OF only works with discrete variables.

>> The code for plotting a CDF of the same sample is as follows:
```python
sample_cdf = thinkstats2.Cdf(sample)
thinkplot.Cdf(sample_cdf)
thinkplot.Config(xlabel='value', ylabel='CDF')
```

>> Which results in the following plot:

![CDF of continuous random values form 0 to 1] (http://i.imgur.com/W7SlYmh.png)
