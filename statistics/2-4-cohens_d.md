[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

I computed Cohen's d using the python code below.

```python
import nsfg
import math


def CohenEffectSize(group1, group2):
    diff = group1.mean() - group2.mean()
    var1 = group1.var()
    var2 = group2.var()
    n1, n2 = len(group1), len(group2)
    pooled_var = (n1 * var1 + n2 * var2) / (n1 + n2)
    d = diff / math.sqrt(pooled_var)
    return d


preg = nsfg.ReadFemPreg()
live = preg[preg.outcome == 1]
firstBabyWeight = live[live.birthord == 1].totalwgt_lb
otherBabiesWeight = live[live.birthord != 1].totalwgt_lb
d = CohenEffectSize(otherBabiesWeight, firstBabyWeight)
print("Cohen d for weight", d)
```

The difference in means for `totalweight_lb` is 0.089 standard deviations, which is small. The is larger compared to the pregnancy length analysis, but a small effect overall.
