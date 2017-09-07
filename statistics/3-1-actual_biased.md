[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

>> I used the following python code:
```python
%matplotlib inline

import numpy as np

import nsfg
import thinkstats2
import thinkplot

resp = nsfg.ReadFemResp()
actual_pmf = thinkstats2.Pmf(resp[].numkdhh)

biased_pmf = actual_pmf.Copy()
for n in actual_pmf:
    biased_pmf.Mult(n,n)
biased_pmf.Normalize()

thinkplot.Pmf(actual_pmf, label = "Actual")
thinkplot.Config(xlabel='Number of Children', ylabel='Pmf')

thinkplot.Pmf(biased_pmf, label = "Biased")
thinkplot.Config(xlabel='Number of Children', ylabel='Pmf')

print (actual_pmf.Mean(), biased_pmf.Mean())
```
>> The "mean of the actual pmf" (really just the sampe average) is 1.02. While that of the "biased pmf" (an estimate of the hypothecial sample average) is: 2.40.
