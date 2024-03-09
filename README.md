# ECMA31350-project
Final project for ECMA 31350 

## Research Topic

The effect of Natural resource abundance/GVC participation rates on political instability 

## Data

Dependent: political instability 

Independent: GVC participation rates by industry sector; mixed, forward, and backward
             Oil Reserves
GVC participation rates: from https://mrio.adbx.online/
   1. https://wits.worldbank.org/gvc/gvc-output-table.html


Controls: log of the share of mountainous land, Ethnic Fractionalization Index, Religion Fractionalization Index, Language Fractionalization Index, the log of population change, legal British origin, log of out-of-region disasters change, demeaned economic growth, and the change in the Democracy Index.


## File description

[`0.1 data_cleaning_gvc.ipynb`]

#### [`stability`]folder

[`0.2 political_stability_data_cleaning.ipynb`]

[`ASPO-Sample.dta`]: political instability data

[`Comprehensive-Sample.dta`]: political instability data

[`Read-me.pdf`]: political instability data codebook

[`stability_df.csv`]: cleaned political instability data

#### [`combined_data`] folder

[`0.3 Data_wrangling.ipynb`]: Data wrangling to merge the data from our 2 data sources and format them properly to be used in our models. 

[`outcome_and_control.ipynb`]: code file to run analysis on initial data/variable selection. 

[`merged_052423.csv`]: the merged WITS eora source gvc data with the stability data, this is our base panel data

[`gvcobp_data.csv`]: merged and wrangled gvc backward data for use in analysis

[`gvcofp_data.csv`]: merged and wrangled gvc forward data for use in analysis

[`gvcomix_data.csv`]: merged and wrangled gvc mixed data for use in analysis



### [`code`] folder

#### [`Baseline_OLS`]

[`2.1 bp_ols.ipynb`]: ols modeling on gvc backward participation data

[`2.2 fp_ols.ipynb`]: ols modeling on gvc forward participation data

[`2.3 mix_ols.ipynb`]: ols modeling on gvc mix participation data

[`2.4 oil_ols.ipynb`]: ols modeling on oil reserves data


#### [`double_ml`]

[`3.1 ml-data-wrangling.ipynb`]: data wrangling for double ml

[`3.2 defense share_plm_mix.ipynb`]: double plm modeling on gvc mixed participation data. 

[`3.3 defense share_plm_forward.ipynb`]: double plm modeling on gvc forward participation data. 

[`3.4 defense share_plm_backward.ipynb`]: double plm modeling on gvc backward participation data. 

[`3.5 defense share_oilreserve.ipynb`]: double plm modeling on oil reserves data. 

[`df_mix.csv`]: double ml gvc mixed participation data.

[`df_fp.csv`]: double ml gvc forward participation data.

[`df_bp.csv`]: double ml gvc backward participation data.

[`mix_res.csv`]: double ml gvc mixed participation modeling results.

[`forward_res.csv`]: double ml gvc forward participation modeling results.

[`backward_res.csv`]: double ml gvc backward participation modeling results.


#### [`Lasso`]

[`4.1 lasso.ipynb`]: lasso for feature selection


#### [`Clustering`]

[`5.1 Clustering_code.ipynb`]：Clustering for measuring regional difference




#### [`Plots`]

[`6.1_plots.ipynb`]: Code for ploting any graphs to use in the paper.

#### [`Summary_stat`]

[`7.1_summary.ipynb`]: Code for summary stats 


[`gvcobp_final_data.csv`]: the same to [`gvcobp_data.csv`] after dropping NAs

[`gvcofp_final_data.csv`]: the same to [`gvcofp_data.csv`] after dropping NAs

[`gvcomix_final_data.csv`]: the same to [`gvcomix_data.csv`]after dropping NAs




