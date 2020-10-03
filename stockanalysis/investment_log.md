## Index ETFs Sharp Ratio
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

## Bond ETFs 
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

## Short Selling
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