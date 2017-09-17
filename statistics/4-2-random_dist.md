[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

def PercentileRank(scores, your_score):
    count = 0
    for score in scores:
        if score <= your_score:
            count += 1

    percentile_rank = 100.0 * count / len(scores)
    return percentile_rank

            
  first_cdf = thinkstats2.Cdf(firsts.totalwgt_lb, label='first')
  other_cdf = thinkstats2.Cdf(others.totalwgt_lb, label='other')
  
  live_cdf.PercentileRank(7.083)
  41.668510732462934
  
  first_cdf.PercentileRank(7.083)
  43.272977309190921
  
