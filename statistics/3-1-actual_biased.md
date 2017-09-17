[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)


pmf = thinkstats2.Pmf(resp.numkdhh, label='actual')

thinkplot.Pmf(pmf)

thinkplot.Config(xlabel = 'Number of Children', ylabel = 'PMF')

>> new_pmf = pmf.Copy(label = 'Biased')

for x, p in new_pmf.Items():

    new_pmf.Mult(x, x)

new_pmf.Normalize()

thinkplot.PrePlot(2)
thinkplot.Pmfs([pmf, new_pmf])
thinkplot.Config(xlabel = 'Number of Chidren', ylabel = 'PMF')

pmf.Mean()
1.0242051550438309

new_pmf.Mean()
2.4036791006642821
