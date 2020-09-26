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
- In this analysis, I first chose some tickers from Bond ETFs that have best price changed in the past 3 months. In the end, I decide to choose ICVT since it has good expected return and high Sharp ratio. This ETF seeks to track the investment results of an index composed of U.S. dollar-denominated convertible securities, specifically cash pay bonds, with outstanding issue sizes greater than $250 million. Here are some facts:
  - Average Yield to Maturity: 1.47%
  - Weighted Avg Maturity: 4.01 yrs
  - Net Assets: $937,990,254
  - Equity Beta (3y): 0.82

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