[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)
>> I used the following code:
```python
import nsfg
preg = nsfg.ReadFemPreg()
firsts = preg[(preg.outcome == 1) & (preg.birthord == 1)].totalwgt_lb
others = preg[(preg.outcome == 1) & (preg.birthord != 1)].totalwgt_lb
pooled = preg[(preg.outcome == 1)].totalwgt_lb

print (firsts.mean() - others.mean())/(pooled.std())
```
>> The calculated effect is .08 standard deviations. That is not huge but it is more than the impact on pregnancy time.
