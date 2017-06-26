[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

>> Of the 2010 Census population, 157.0 million were female (50.8 percent) while 151.8 million were male (49.2 percent). (https://www.census.gov/prod/cen2010/briefs/c2010br-03.pdf)
The code to answer the question "How many people are between 5'10'' and 6'1''?" is as follows:

```python
import scipy.stats

US_male_percent = (dist.cdf(185.42) - dist.cdf(177.8))*100
US_males = (dist.cdf(185.42) - dist.cdf(177.8))*151800000
print(int(US_male_percent), 'percent of male population in US is eligible to join Blue Man Group')
print(int(US_males), 'males in US are eligible to join Blue Man Group')
```
>> The above script returns the following:

```
34 percent of male population in US is eligible to join Blue Man Group
52028969 males in US are eligible to join Blue Man Group
```
