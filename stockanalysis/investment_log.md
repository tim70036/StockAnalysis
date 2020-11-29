## Index ETFs Sharp Ratio (Week1)
- The ETF I select is IBUY. It corresponds generally to the price performance of the EQM Online Retail Index. This Index is a basket of companies that obtain 70% or more of revenue from online or virtual sales. The expense ratio is 0.65%.

- I set the time period of my analysis from 2020-4-9 to 2020-9-23. The reason I choose this period is that I want to see which stock has good performance after COVID crash. Then, I calculate sharp ratios from the stocks in my regular watchlist. The result shows that IBUY has the highest sharp ratio 0.312674 during this period. Also, the SP500 sharp ratio is 0.115277, so IBUY clearly outperform SP500 in this period.

- Provided data below:
    ```
    SP500  sharp: 0.115277
    IBUY   sharp: 0.312674 || relative_sharp: 0.191306
    ARKF   sharp: 0.280109 || relative_sharp: 0.158741
    ARKW   sharp: 0.255015 || relative_sharp: 0.133647
    ESPO   sharp: 0.241484 || relative_sharp: 0.120116
    TAN    sharp: 0.237422 || relative_sharp: 0.116055
    ARKK   sharp: 0.235704 || relative_sharp: 0.114336
    ARKG   sharp: 0.201813 || relative_sharp: 0.080445
    XRT    sharp: 0.200940 || relative_sharp: 0.079573
    ...
    ```

## Bond ETFs (Week2)
- In this analysis, I first chose some tickers from Bond ETFs that have best price changed in the past 3 months. In the end, I decide to choose CWB since it has good expected return and high Sharp ratio. This ETF seeks to provide investment results that, before fees and expenses, correspond generally to the price and yield performance of the Bloomberg Barclays US Convertible Liquid Bond Index. This index represent the market of U.S. convertible securities, such as convertible bonds. Here are some facts:
  - Gross Expense Ratio: 0.4%
  - Current Yield: 1.94%
  - Weighted Avg Maturity: 4.41 yrs
  - Net Assets: $4,928.32 M

- After getting 10 years data, We can see that bond ETFs generally have lower mean and standard deviation on return than SP500. This is reasonable since the volatility of bond is smaller than stocks. The only exception in the data is Covertible Bond ETF. They have high mean and standard deviation almost same as SP500. That's probably because they can convert to stocks and thus behave more like stocks.

- To evaluate performace, we look at their sharp ratio. It turns out that some bonds have better performance over SP500. Below is the statistics of the bond ETFs that has higher Sharp ratio than SP500 (the last row is SP500):
    ```
    Getting data 2010-08-31 00:00:00 -> 2020-09-01 00:00:00
    ^GSPC NUAG CBON BND VCSH TIP VCIT HYLB KCNY IUSB HYLD HYXU NEAR IGLB LQD SHY IEF TLT ICVT CWB PFF 
    Sorted by sharp ratio:
    VCIT   mean: 0.020879%  std: 0.341645%  sharp: 0.054505
    CWB    mean: 0.044660%  std: 0.797649%  sharp: 0.052718
    VCSH   mean: 0.011651%  std: 0.188412%  sharp: 0.050389
    ICVT   mean: 0.050866%  std: 1.028362%  sharp: 0.045993
    IUSB   mean: 0.015409%  std: 0.261715%  sharp: 0.045586
    BND    mean: 0.013945%  std: 0.270118%  sharp: 0.044684
    LQD    mean: 0.021567%  std: 0.457141%  sharp: 0.042864
    ^GSPC  mean: 0.047859%  std: 1.092130%  sharp: 0.042609
    ```

- On the other hand, if we only look at 5 years data, we can see that SP500 has worse Sharp ratio than 10 years. However, the bonds ETF remain their high Sharp ratio. Also, the number of bonds that outperform SP500 increases. This shows us in the past 5 years some bond ETFs perform better than overall stock market. The mean and standard deviation remain similar. Below is the statistics of the bond ETFs that has higher Sharp ratio than SP500 (the last row is SP500):
    ```
    Getting data 2015-08-31 00:00:00 -> 2020-09-01 00:00:00
    ^GSPC NUAG CBON BND VCSH TIP VCIT HYLB KCNY IUSB HYLD HYXU NEAR IGLB LQD SHY IEF TLT ICVT CWB PFF 
    Sorted by sharp ratio:
    CWB    mean: 0.054362%  std: 0.924893%  sharp: 0.054129
    ICVT   mean: 0.059239%  std: 1.044036%  sharp: 0.053197
    VCIT   mean: 0.023661%  std: 0.373421%  sharp: 0.052245
    IUSB   mean: 0.016914%  std: 0.265389%  sharp: 0.048594
    BND    mean: 0.017463%  std: 0.314600%  sharp: 0.041606
    LQD    mean: 0.026226%  std: 0.539107%  sharp: 0.041461
    IEF    mean: 0.018081%  std: 0.343476%  sharp: 0.040555
    TIP    mean: 0.017244%  std: 0.332737%  sharp: 0.040023
    VCSH   mean: 0.013290%  std: 0.239087%  sharp: 0.038659
    IGLB   mean: 0.033470%  std: 0.780001%  sharp: 0.038032
    SHY    mean: 0.006812%  std: 0.066376%  sharp: 0.037768
    ^GSPC  mean: 0.045569%  std: 1.210576%  sharp: 0.036170
    ```

- In my opinion, I prefer 5 years data over 10 years. Since in recent years, stock and bond market showed increased volatility (especially after 2018). Under such unprecedented circumstances, it's better to use more recent data to reflect the performance of each asset.

## Short Selling (Week3)
- If I short a bond that means I think that interest rate might go up in the future. If I short a stock, that means I think that company will not do well in the future or the stock is in fomo buying now.

- I gather the data from my watchlist, it contains ETFs from different sector and also ETFs in bond and agriculture. I set the time period of my analysis from 2020-4-9 to 2020-9-23. The reason I choose this period is that I want to see which stock has worst performance after COVID crash. Data from 10yrs long period might not give me enough insight on how COVID has changed the world. The result is shown below:
```
Getting data 2020-04-09 00:00:00 -> 2020-10-03 00:00:00
^GSPC IVV QQQ IJR IJH SHY IEF TLT JETS VGT CLOU XBI XPH XLV XLP XLY XRT ITB XLF KRE XLI IYT ITA XLE XOP VNQ XLU XLB XME DBA CORN SOYB WEAT 
Sorted by the percentage of negative log returns in all windows:
XLE    rolling_mean: -0.029255% rolling_neg_pct: 73.170732%
XOP    rolling_mean: -0.004161% rolling_neg_pct: 63.414634%
TLT    rolling_mean: 0.001060% rolling_neg_pct: 53.658537%
WEAT   rolling_mean: 0.003819% rolling_neg_pct: 39.024390%
CORN   rolling_mean: 0.018614% rolling_neg_pct: 37.804878%
IEF    rolling_mean: 0.003190% rolling_neg_pct: 35.365854%
XBI    rolling_mean: 0.065458% rolling_neg_pct: 34.146341%
KRE    rolling_mean: 0.033262% rolling_neg_pct: 34.146341%
ITA    rolling_mean: 0.034101% rolling_neg_pct: 28.048780%
XLU    rolling_mean: 0.019002% rolling_neg_pct: 28.048780%
DBA    rolling_mean: 0.032655% rolling_neg_pct: 24.390244%
JETS   rolling_mean: 0.097821% rolling_neg_pct: 20.731707%
XLV    rolling_mean: 0.033413% rolling_neg_pct: 20.731707%
XPH    rolling_mean: 0.029221% rolling_neg_pct: 17.073171%
XLF    rolling_mean: 0.049673% rolling_neg_pct: 17.073171%
VNQ    rolling_mean: 0.043682% rolling_neg_pct: 15.853659%
IJR    rolling_mean: 0.082565% rolling_neg_pct: 13.414634%
IJH    rolling_mean: 0.075944% rolling_neg_pct: 9.756098%
SHY    rolling_mean: 0.000599% rolling_neg_pct: 8.536585%
XLP    rolling_mean: 0.053406% rolling_neg_pct: 8.536585%
SOYB   rolling_mean: 0.049635% rolling_neg_pct: 4.878049%
XME    rolling_mean: 0.118317% rolling_neg_pct: 3.658537%
CLOU   rolling_mean: 0.127869% rolling_neg_pct: 2.439024%
XLI    rolling_mean: 0.100097% rolling_neg_pct: 2.439024%
XLB    rolling_mean: 0.103104% rolling_neg_pct: 1.219512%
^GSPC  rolling_mean: 0.076560% rolling_neg_pct: 0.000000%
IVV    rolling_mean: 0.079636% rolling_neg_pct: 0.000000%
QQQ    rolling_mean: 0.117742% rolling_neg_pct: 0.000000%
VGT    rolling_mean: 0.120661% rolling_neg_pct: 0.000000%
XLY    rolling_mean: 0.116691% rolling_neg_pct: 0.000000%
XRT    rolling_mean: 0.163313% rolling_neg_pct: 0.000000%
ITB    rolling_mean: 0.201578% rolling_neg_pct: 0.000000%
IYT    rolling_mean: 0.143020% rolling_neg_pct: 0.000000%
---------------------------------------------------------
```

- From looking at the result, I decide to short XLE, which has the highest negative percentage in all windows. Besides from the result, we all know that COVID has shut down the world. This also caused the demand for energy and oil declined significantly. Unless the vaccine come out, it's almost impoosible that the world will re-open and move the demand for energy back to normal. As a result, I think XLE is not gonna do well in the following months.


## Leveraged (Week4)

- I gather the data from my watchlist, it contains ETFs from different sector and also ETFs in bond and agriculture. The normal stats:
```
Getting data 2018-10-10 00:00:00 -> 2020-10-11 00:00:00
^GSPC IVV QQQ IJR IJH SHY IEF TLT JETS VGT CLOU XBI XPH XLV XLP XLY XRT ITB XLF KRE XLI IYT ITA XLE XOP VNQ XLU XLB XME DBA CORN SOYB WEAT 
Sorted by sharp ratio:
SHY    mean: 0.015068%  std: 0.078735%  sharp: 0.118181
IEF    mean: 0.045133%  std: 0.395094%  sharp: 0.097811
CLOU   mean: 0.143021%  std: 2.053841%  sharp: 0.066919
TLT    mean: 0.076049%  std: 1.077496%  sharp: 0.063227
VGT    mean: 0.105020%  std: 2.031529%  sharp: 0.052235
QQQ    mean: 0.095039%  std: 1.847045%  sharp: 0.051916
ITB    mean: 0.117372%  std: 2.581462%  sharp: 0.044079
XLY    mean: 0.067330%  std: 1.724949%  sharp: 0.038267
XLP    mean: 0.049868%  std: 1.356419%  sharp: 0.034876
IVV    mean: 0.045023%  std: 1.694545%  sharp: 0.026830
XLU    mean: 0.044095%  std: 1.793120%  sharp: 0.025620
XLB    mean: 0.043932%  std: 1.869289%  sharp: 0.024383
^GSPC  mean: 0.037361%  std: 1.693221%  sharp: 0.022548
XBI    mean: 0.061254%  std: 2.306989%  sharp: 0.022337
XLV    mean: 0.035342%  std: 1.532521%  sharp: 0.022070
VNQ    mean: 0.023143%  std: 1.991610%  sharp: 0.011744
XRT    mean: 0.028328%  std: 2.042677%  sharp: 0.010930
XLI    mean: 0.015433%  std: 1.933643%  sharp: 0.008904
IYT    mean: 0.017265%  std: 2.011804%  sharp: 0.008141
IJH    mean: 0.010744%  std: 1.985204%  sharp: 0.005591
XPH    mean: 0.009589%  std: 1.775305%  sharp: 0.000721
SOYB   mean: 0.001838%  std: 0.868700%  sharp: -0.005899
XLF    mean: -0.011978%  std: 2.134997%  sharp: -0.006318
IJR    mean: -0.012041%  std: 2.062300%  sharp: -0.006937
XME    mean: -0.047133%  std: 2.412697%  sharp: -0.018813
ITA    mean: -0.045611%  std: 2.249113%  sharp: -0.020278
WEAT   mean: -0.016952%  std: 1.365022%  sharp: -0.024948
KRE    mean: -0.069761%  std: 2.755435%  sharp: -0.026355
JETS   mean: -0.097793%  std: 3.055029%  sharp: -0.034138
DBA    mean: -0.025130%  std: 0.802368%  sharp: -0.045075
CORN   mean: -0.035684%  std: 1.073479%  sharp: -0.045203
XLE    mean: -0.158949%  std: 2.725159%  sharp: -0.055006
XOP    mean: -0.262833%  std: 3.845893%  sharp: -0.064454
---------------------------------------------------------
```

- Then I calculate the leveraged investment stats using 4:1 ratio and considering borrowing cost:
```
Getting 4:1 leveraged data 2018-10-10 00:00:00 -> 2020-10-11 00:00:00
^GSPC IVV QQQ IJR IJH SHY IEF TLT JETS VGT CLOU XBI XPH XLV XLP XLY XRT ITB XLF KRE XLI IYT ITA XLE XOP VNQ XLU XLB XME DBA CORN SOYB WEAT 
Sorted by sharp ratio:
IEF    mean: 0.146839%  std: 1.587003%  sharp: 0.092526
SHY    mean: 0.028933%  std: 0.315764%  sharp: 0.091629
CLOU   mean: 0.542229%  std: 8.246566%  sharp: 0.065752
TLT    mean: 0.265305%  std: 4.328648%  sharp: 0.061291
VGT    mean: 0.417342%  std: 8.150052%  sharp: 0.051207
QQQ    mean: 0.376211%  std: 7.407807%  sharp: 0.050786
ITB    mean: 0.448617%  std: 10.367689%  sharp: 0.043271
XLY    mean: 0.256521%  std: 6.922252%  sharp: 0.037057
XLP    mean: 0.180716%  std: 5.421898%  sharp: 0.033331
IVV    mean: 0.173877%  std: 6.792889%  sharp: 0.025597
XLU    mean: 0.175207%  std: 7.165661%  sharp: 0.024451
XLB    mean: 0.174397%  std: 7.495890%  sharp: 0.023266
XBI    mean: 0.198684%  std: 9.269808%  sharp: 0.021433
^GSPC  mean: 0.144626%  std: 6.785751%  sharp: 0.021313
XLV    mean: 0.127199%  std: 6.142987%  sharp: 0.020706
VNQ    mean: 0.085292%  std: 7.975889%  sharp: 0.010694
XRT    mean: 0.081349%  std: 8.209133%  sharp: 0.009910
XLI    mean: 0.060638%  std: 7.751379%  sharp: 0.007823
IYT    mean: 0.057325%  std: 8.070041%  sharp: 0.007103
IJH    mean: 0.036135%  std: 7.962223%  sharp: 0.004538
XPH    mean: -0.003234%  std: 7.132370%  sharp: -0.000453
XLF    mean: -0.062536%  std: 8.571696%  sharp: -0.007296
IJR    mean: -0.065831%  std: 8.282317%  sharp: -0.007948
SOYB   mean: -0.028945%  std: 3.486088%  sharp: -0.008303
XME    mean: -0.190547%  std: 9.683184%  sharp: -0.019678
ITA    mean: -0.191354%  std: 9.023362%  sharp: -0.021206
WEAT   mean: -0.144482%  std: 5.455394%  sharp: -0.026484
KRE    mean: -0.300129%  std: 11.070003%  sharp: -0.027112
JETS   mean: -0.427140%  std: 12.266807%  sharp: -0.034821
CORN   mean: -0.201881%  std: 4.280746%  sharp: -0.047160
DBA    mean: -0.153104%  std: 3.210661%  sharp: -0.047686
XLE    mean: -0.608860%  std: 10.916648%  sharp: -0.055774
XOP    mean: -1.002324%  std: 15.421022%  sharp: -0.064997
---------------------------------------------------------
```

- Compare these 2 set of data, we can see that leveraged stat has almost 4x expected return and standard deviation than normal stats. It's not exactly 4x due to the borrowing cost. The borrowing cost also cause the leveraged investment to have worse sharp ratio than normal one.

- After examining these results, I decide to choose CLOU. This is because it has better sharp ratio compare to SP500 and has the best among all non-bond ETFs. Also, CLOU invest in companies positioned to benefit from the increased adoption of cloud computing technology, including companies whose principal business is in offering computing Software-as-a-Service (SaaS), Platform-as-a-Service (PaaS), Infrastructure-as-a-Service (IaaS), managed server storage space and data center real estate investment trusts, and/or cloud and edge computing infrastructure and hardware. After COVID crash, CLOU has benefit from the remote working trend and the digitalize trend all over the world. As a result, I believe CLOU is a good investment and I use leveraged investment to get a mega boost.

## Small Cap (Week5)

- I choosed some ETFs on the small cap list and get the following data:
```
Getting data 2010-08-31 00:00:00 -> 2020-10-18 00:00:00
^GSPC VBK VBR IJH SCHA IWO IJJ SPMD XMLV SLY 
Sorted by sharp ratio:
^GSPC  mean: 0.047055%  std: 1.096562%  sharp: 0.041709
VBK    mean: 0.056642%  std: 1.323329%  sharp: 0.040658
IWO    mean: 0.053971%  std: 1.409595%  sharp: 0.035599
IJH    mean: 0.045780%  std: 1.272892%  sharp: 0.034092
SCHA   mean: 0.046093%  std: 1.343458%  sharp: 0.032211
XMLV   mean: 0.036407%  std: 1.071656%  sharp: 0.031436
SLY    mean: 0.045812%  std: 1.355165%  sharp: 0.030397
VBR    mean: 0.039676%  std: 1.321365%  sharp: 0.028173
IJJ    mean: 0.039144%  std: 1.328737%  sharp: 0.027817
SPMD   mean: 0.020331%  std: 1.307305%  sharp: 0.013215
---------------------------------------------------------

Getting data 2020-04-09 00:00:00 -> 2020-10-18 00:00:00
^GSPC VBK VBR IJH SCHA IWO IJJ SPMD XMLV SLY 
Sorted by sharp ratio:
VBK    mean: 0.286212%  std: 1.616716%  sharp: 0.176764
IWO    mean: 0.287931%  std: 1.850204%  sharp: 0.155386
^GSPC  mean: 0.177844%  std: 1.378049%  sharp: 0.128740
SCHA   mean: 0.245789%  std: 1.974191%  sharp: 0.124281
IJH    mean: 0.203337%  std: 1.857329%  sharp: 0.109243
SPMD   mean: 0.202346%  std: 1.861854%  sharp: 0.108446
SLY    mean: 0.208531%  std: 2.247893%  sharp: 0.092574
VBR    mean: 0.191616%  std: 2.165853%  sharp: 0.088270
IJJ    mean: 0.169288%  std: 2.183945%  sharp: 0.077316
XMLV   mean: 0.039679%  std: 1.571214%  sharp: 0.024977
---------------------------------------------------------
```

- When computing, I choose 2 periods: past 10 year data and data after COVID crash. In past 10 years, small cap ETFs had worse sharp ratio than SP500 and only few of them have better expected return than SP500. However, after COVID crash, there were 2 ETFs standing out. We can see that VBK perform well in both periods. It even had better Sharp ratio than SP500 after COVID crash this year. As a result, I decide to long VBK in this week strategy.


## Value investing (Week6)

- For SP500: PB ratio 3.437, PE ratio 26.65, Dividend yield 1.75%.

- Among the large cap stocks, I choose Cisco Systems Inc CSCO. It has: PB ratio 4.32, PE ratio 14.7, Dividend yield 5.35%. CSCO has relative low PE ratio compare to SP500. This shows its price is undervalued given a good earning. Also, the dividend yield is quite high. On the other hand, PB ratio of CSCO is hihger than SP500. However, here I choose to look at PE and Dividend Yield, since I want to see how well the company peform (earning) instead of how healthy(asset) the company is.

- One of my existing investment is Zoom ZM. It has: PB ratio 121.36, PE ratio 647.49, no dividend yield. We can see that the number is high and ZM is cleary overvalued compare to SP500 or CSCO. The high price is due to everyone expects it'll grow pretty fast in the near future. Thus, growth stock is very different from value stock such as CSCO.

## Momentum Strategies (Week7)

- I choose [XOP, JKS, JETS, ZM, FB] as candidates. The period I observe starts after COVID crash 4/9/2020 to 10/31/2020. Here is the return for each candidate:
```
XOP: -0.7%
JKS: 281.05%
JETS: 10.59%
ZM: 270.18%
FB: 50.19%
```

- Given this, I decide to long JKS and short XOP. The differnece of return between these 2 assets is 281.75%.

## Final

- The week1 strategy gives the best performance. IBUY ETF gives me 11.19% of return. It has thr best sharp ratio among a list of ETFs compare to SP500 after COVID crash, and I think that's why it gives a good performance. I do think it's a superior strategy compare to other weeks strategy since I'm choosing ETFs from different industry. Instead of suffering more uncertainty from individual stocks, ETFs could give me less variance on return. Also, stock ETFs could give me more return than bond ETFs. Especially, the bond price right now is too high due to low interest rate. As a result, I think the ETF I choose should have a high probablity to give me the best result among all strategies.

- The week3 strategy gives the worst performance (-14.58%). The reason why it does is because the vaccine news. Given that the whole world would shut down for a while, XLE has been performing really bad. After I short it, it did give me some positive return. However, it suddenly jumped up on 11/9 due to Pfizer vaccine news. Nevertheless, I still think the decision I made is correct. Just have to work on choosing better timing.

- I learned a lot from these weekly project. I really enjoy crawling down market data and make some calculation on them. Also, the project gives me an idea how real world investing works.