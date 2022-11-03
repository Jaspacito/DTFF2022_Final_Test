# DTFF2022_Final_Test



## Deadline and Timetable 

Deadline: *2022-12-19* 

10-31 ~ 11-06: 

11-07 ~ 11-13: 

11-14 ~ 11-20: 

11-21 ~ 11-27: 

11-28 ~ 12-04: 

12-05 ~ 12-11: 

12-12 ~ 12-18: 

## Data
1. Inflation Rate: monthly year-on-year CPI data with the logarithm form released by the National Bureau of Statistics, sample period: 01.2010 - 03.2014.

   https://data.stats.gov.cn/easyquery.htm?cn=A01&zb=A010201&sj=202210

2. Expected Inflation rate: proxied by the one period lagged one-year national bond’s yield to maturity, obtained from the China Government Securities Depository Trust &Clearing Co. Ltd., sample period: 01.2010 - 03.2014.

   https://www.cbirc.gov.cn/cn/view/pages/index/guozhai.html

3. Commodity Futures： sixteen kinds of future contracts from the Shanghai, Dalian, Zhengzhou futures exchange:  Soybeans No. 1, soybeans No. 2, yellow corn, LLDPE, soybean meal, palm oil, soybean oil, PVC, cathode copper, aluminum, zinc, gold, natural rubber, fuel oil, rebar, wire rod. Use the settlement price namely the market volume weighted strike price of the contract to calculate their return. Considering that the CPI is monthly data, to match the data frequency, we selected the settlement price at the end of each month to calculate the one-year holding period returns. In addition, due to commodity futures can be short, they have more advantages over stocks. Sample period: 01.2010 - 03.2014.

   https://www.shfe.com.cn/statements/dataview.html?paramid=delaymarket_bc

   http://www.dce.com.cn/dalianshangpin/xqsj/tjsj26/rtj/yxq/index.html

4. Real estate returns are calculated based on the housing price index in the first-tier cities, second-tier cities and third-tier cities, which are released by the China Index Academy. Sample period: 06.2011 - 03.2014.

6. The gold return is obtained from the closing price of spot gold from Shanghai Gold Exchange, sample period: 01.2010 - 03.2014.

7. Industry Stocks: the closing price of Hushen 300 industry Index at the end of each month to calculate the one-year holding period yield, the included industries are energy, raw materials, industry, optional consumption, the main consumption, medicine and health care, finance and real estate, information technology, the utility and the telecommunication service, sample period: 01.2010 - 03.2014.




## To Do List based on Requirements and Literature 

1. Single repository on GitHub, all group members as controbutor 

- check contributors，repo finished 

2. Neatly and concisely structure 

- use Cookiecutter 

3. Keep working on it consistently, avoid bulk commits

- use test repo first, officially commit maybe once a week 

4. Create well-documented database, with update methods

- use Docker tocreate and manage database would have extra bonus 

5. Design figures and tables, with visualization standards discussed in class

- class to be taken 

6. Short paper using LaTeX or Jupyter/Shiny, populating it with sections, a table of contents, and the above tables and figures 

- to be determined how to do 

7. A beamer presentation for project using LaTeX

- what is 'beamer presentation'? 

8. One interactive app (Shiny or Jupyter notebook) describing the main finding and presenting several robustness checks

- class to be taken 

9. Results are reproducible by ensuring that the coding environment is exported and concise documentation is present

- to be determined how to do 



## Official Requirements for Final Project 

(75\%, group assignment, same grade, deadline 19-Dec-2022)

Please submit a little research project adhering to the following requirements:

- make it hosted as a single repository on Github with all group members as contributors;
- structure it neatly and concisely, avoid the clutter of folders and files for which third people have no use (use .gitignore);
- keep working on it consistently, avoid bulk commits;
- create a little well-documented database with the data you use, ideally with update methods;
- design figures and tables to support your findings, keeping them in line with visualization standards discussed in class;
- write a short paper about it using LaTeX or Jupyter/Shiny, populating it with sections, a table of contents, as well as the above tables and figures;
- write a beamer presentation for your project using LaTeX;
- create one interactive app (Shiny or Jupyter notebook) describing the main finding and presenting several robustness checks;
- make sure the results are reproducible by ensuring that the coding environment is exported and concise documentation is present;
- in the ideal case, anyone who could pass this course should be able to see and reproduce your findings from scratch.

You can pick a topic from the [list of suggested topics](./research-topics.md), but own topics are strongly encouraged! You can also choose to replicate a result from a paper (which does not have an open-source implementation yet).


