[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

>> Below is the code I used:
```python
import random
import thinkstats2

rand = []
for i in range(1000):
    rand.append(random.random())

rand_pmf = thinkstats2.Pmf(rand)
thinkplot.Pmf(rand_pmf, label = "Random.Random")
thinkplot.Config(xlabel='number', ylabel='Pmf')

rand_cdf = thinkstats2.Cdf(rand)
thinkplot.Cdf(rand_cdf, label = "Random.Random")
thinkplot.Config(xlabel='number', ylabel='prob')
```
>> Below are the graphs:

![Actual pmf](../img/rand_pmf.png?raw=true )
![Biased pmf](../img/rand_cdf.png?raw=true )

>> It looks pretty uniform to me.
