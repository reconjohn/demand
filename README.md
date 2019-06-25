## R package: demand

This package creates diverse plots per day, weekday, month and year for peak demand power consumption of several meters to support a [project, demand_acep](https://github.com/demand-consults/demand_acep), which was developed to make raw data of electricity consumption of 4 meters in Poker Flat Research Range (PRFR) ready to use for the further analyses. These plots lead to benefit-cost analyses and cost saving plots based on [electricity rate structure from GVEA](http://www.gvea.com/rates/rates) in Alaska. 

> Poker Flat Research Range (PFRR) is located about 40 miles North of Fairbanks, AK and serves as a sounding rocket launch facility and for other geophysical research activities. PFRR is operated by the University of Alaska Fairbanks (UAF) under contract with NASA. 


<table class="table table-striped table-hover table-condensed" style="margin-left: auto; margin-right: auto;">
<caption>Rate schedule</caption>
 <thead>
  <tr>
   <th style="text-align:left;"> Service Type </th>
   <th style="text-align:right;"> Customer Charge [$/month] </th>
   <th style="text-align:right;"> Utility Charge [$/kWh] </th>
   <th style="text-align:right;"> Fuel &amp; Purchased Power Charge [$/kWh] </th>
   <th style="text-align:right;"> Demand Charge [$/kW] </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:left;"> Residential </td>
   <td style="text-align:right;"> 17.5 </td>
   <td style="text-align:right;"> 0.11631 </td>
   <td style="text-align:right;"> 0.09207 </td>
   <td style="text-align:right;"> 0.00 </td>
  </tr>
  <tr>
   <td style="text-align:left;"> GS-1 </td>
   <td style="text-align:right;"> 20.0 </td>
   <td style="text-align:right;"> 0.11528 </td>
   <td style="text-align:right;"> 0.09207 </td>
   <td style="text-align:right;"> 0.00 </td>
  </tr>
  <tr>
   <td style="text-align:left;"> GS-2(S) </td>
   <td style="text-align:right;"> 30.0 </td>
   <td style="text-align:right;"> 0.06256 </td>
   <td style="text-align:right;"> 0.09207 </td>
   <td style="text-align:right;"> 14.29 </td>
  </tr>
  <tr>
   <td style="text-align:left;"> GS-2(P) </td>
   <td style="text-align:right;"> 30.0 </td>
   <td style="text-align:right;"> 0.06256 </td>
   <td style="text-align:right;"> 0.09207 </td>
   <td style="text-align:right;"> 14.29 </td>
  </tr>
  <tr>
   <td style="text-align:left;"> GS-3 </td>
   <td style="text-align:right;"> 295.0 </td>
   <td style="text-align:right;"> 0.02940 </td>
   <td style="text-align:right;"> 0.09207 </td>
   <td style="text-align:right;"> 22.86 </td>
  </tr>
</tbody>
</table>


In addition, this package forecasts peak power demand using ARIMA on a daily and monthly basis. Correlation and a simple regression are also included. 



To use ths package, follow the steps:

1. Install `devtools`
```
install.packages("devtools")
```

2. Load the package 
```
library(devtools)
```

3. Install this package `demand`
```
install_github("reconjohn/demand")
```

3. Load the package 
```
library(demand)
```

Now you are all set!

## Brief description of demand charge using R package, `demand`

Using R package `demand`, peak demand, correlation, forecast, and demand charge were plotted. Refer to the followings for more details about demonstration of code from `demand` package and its results. 

* Peak demand plot for the 4 meters  [here](https://github.com/demand-consults/demand_acep/blob/master/demand/scripts/plots.md) and 
[code](https://github.com/demand-consults/demand_acep/blob/master/demand/scripts/plots.Rmd)

* Peak demand correlation and forecasts [here](https://github.com/demand-consults/demand_acep/blob/master/demand/scripts/forecast.md) and 
[code](https://github.com/demand-consults/demand_acep/blob/master/demand/scripts/forecast.Rmd)

* Demand charge reduction by implementing a virtual meter [here](https://github.com/demand-consults/demand_acep/blob/master/demand/scripts/charge_filled.md) and
[code](https://github.com/demand-consults/demand_acep/blob/master/demand/scripts/charge_filled.Rmd)


## Examples are as follows: 

### Peak demand (kW) plot of day per month
![](./scripts/plots_files/figure-html/unnamed-chunk-1-1.png)

### ARIMA forecast for predicting 10 days
![](./scripts/forecast_files/figure-html/unnamed-chunk-24-1.png)

### ARIMA forecast for predicting 3 months
![](./scripts/forecast_files/figure-html/unnamed-chunk-12-1.png)

### Peak demand comparison between a virtual meter and the 4 meters 
![](./scripts/charge_filled_files/figure-html/unnamed-chunk-1-1.png)

### Cost comparison and saving 
![](./scripts/charge_filled_files/figure-html/unnamed-chunk-7-1.png)

### Monthly saving distribution 
![](./scripts/charge_filled_files/figure-html/unnamed-chunk-8-1.png)


View the project [here](https://github.com/demand-consults/demand_acep).

---

To the extent possible under law,
[Yohan Min](https://github.com/reconjohn)
has waived all copyright and related or neighboring rights to
&ldquo;[R package demand](https://github.com/reconjohn/demand)&rdquo;.
This work is published from the United States.
