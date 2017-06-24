[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

>> Following guidelines from chap03ex.ipynb, I have come up with the following code:  
`
import thinkstats2  
import nsfg  
import thinkplot  
`
`
resp = nsfg.ReadFemResp()  
resp_pmf = thinkstats2.Pmf(resp.numkdhh, label='actual')  
biased_resp_pmf = BiasPmf(resp_pmf, label='observed')  
thinkplot.PrePlot(2)  
thinkplot.Pmfs([resp_pmf, biased_resp_pmf])  
thinkplot.Config(xlabel='Number of children in family', ylabel='PMF')  
print('Unbiased Mean:', resp_pmf.Mean())  
print('Biased Mean:', biased_resp_pmf.Mean())  
`

>> The obtained result was as follows:

`
Unbiased Mean: 1.02420515504  
Biased Mean: 2.40367910066
`  
![Biased/Unbiased PMF Comparison](http://i.imgur.com/k1kHLs6.png)
