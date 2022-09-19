# Accessing Macro and Factors Data

The repository shows how to import different open source financial data sets and macroeconomic time series to formulate hypotheses and develop investment insights.

## Project Description

First, load the needed packages for web scrapping tasks.

Second, import the different factors data sets from [AQR](https://www.aqr.com/Insights/Datasets?&page=1#filtered-list) website and modify the format of some variables to facilitate the consolidation of the different factors data sets into one. Then, store the resulting dataset.

Third, import the different macroeconomic data sets from [FRED](https://fred.stlouisfed.org/) website and modify the format of some variables to facilitate the consolidation of the different factors data sets into one. Then, store the resulting dataset. 

## Usage
The resulting datasets can be used to infer what is the current macroeconomic regime, what is the trend in certain macroeconomic variables, test the relationship between macro variables and investment factors, and monitor the investment performance of the investment factors included in the data set.

```python
# what is the YTD accumulated value of $100 investment on each investment factor?
data[-8:].add(1).cumprod().mul(100).normalize().iplot(kind='lines', theme='polar', title='Factors Commulative Return YTD',  yTitle='$')

```
## Author
Martin Escobar
LinkedIn: [mescobars](https://www.linkedin.com/in/mescobars/)
Twitter: [@m_escobars](https://twitter.com/m_escobars)

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
