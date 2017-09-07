[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

>> I used the following code:
```python
import scipy

def z_score(raw):
    return (raw - 178) / 7.7

upper_cm = (6*12 + 1)*2.54
lower_cm = (5*12 + 10)*2.54

print scipy.stats.norm.cdf(z_score(upper_cm), z_score(lower_cm))
```
>> The answer I found was 83.9%.

