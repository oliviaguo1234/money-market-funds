This project analyzes data of money market funds to evaluate how primary manager, regulatory category, and public listing status impact funds and behaviors in the U.S. Money Market Funds sector. To this end, it combines econometrics, hypothesis tests, and machine learning to predict fund categories.
The Herfindahl–Hirschman index (HHI) was used to measure market concentration.

### Key Findings:
* While the overall MMF market is unconcentrated ($\text{HHI} = 607.78$), specific sub-markets are exceptions. Single State municipal funds are relatively uncompetitive ($\text{HHI} = 2885.33$), exceeding the Department of Justice (DOJ) benchmark for high concentration ($2,500$).
* A chi-square test revealed how manager size was strongly correlated with usage of sub-advisors ($\chi^2 = 220.44, p < 0.001$), with a strong overall effect (Cramer's $V = 0.428$).
* Tier 1 (Large-Sized): tend to rely on sub-advisors ($\text{Residual} = +8.68$)
* Tier 2 (Medium-Sized): demonstrate strong internalization ($\text{Residual} = -8.55$)
* A one-way ANOVA test with Tukey's HSD confirmed statistically significant differences in share class density across different categories ($p < 0.001$), with government funds shown to have significantly fewer share classes than Prime ($p = 0.01$) and Other Tax-Exempt funds ($p = 0.023$).
* A Mann-Whitney U Test demonstrated how publicly listed funds ('has_class_ticker_symbol = 1') had significantly higher class density.
* A Random Forest Classifier with ~78.5% predictive accuracy was able to identify share class density as a very important indicator.
