# DTFF2022_Final_Test



## Deadline and Timetable 

Deadline: *2022-12-19* 

10-31 ~ 11-09: 

 - collect all the deta needed 

11-10 ~ 11-16: 

 - upload data files to ./data folder 
 - read the literature, be familiar with the model used in literature, and confirm the methodology of data precessing 

11-17 ~ 11-23: 

 - None 

11-24 ~ 11-30: 

 - None 

12-01 ~ 12-07: 

 - Database：construct database by cuckiecutter，import data to database，update data 
 - Section 2.2 Data: compute monthly year-on-year log return 
 - Section 2.3.1 Stationary Test 
 - Section 2.3.2 ~ 2.3.4 Hedging Effect Test 
 - Section 3 Porfolio Construction 

12-08 ~ 12-14: 

12-15 ~ 12-18: 

## Data
1. Inflation Rate: monthly year-on-year CPI data with the logarithm form released by the National Bureau of Statistics, sample period: 01.2010 - 03.2014.

   https://data.stats.gov.cn/easyquery.htm?cn=A01&zb=A010201&sj=202210 
   
   ***2009-12 ~ 2010-12 数据缺失*** 

2. Expected Inflation rate: proxied by the one period lagged one-year national bond’s yield to maturity, obtained from the China Government Securities Depository Trust &Clearing Co. Ltd., sample period: 01.2010 - 03.2014.

   https://www.cbirc.gov.cn/cn/view/pages/index/guozhai.html
   
   ***2009-12 数据缺失*** 

3. Commodity Futures： sixteen kinds of future contracts from the Shanghai, Dalian, Zhengzhou futures exchange:  Soybeans No. 1（豆一）, soybeans No. 2（豆二）, yellow corn（玉米）, LLDPE（聚乙烯）, soybean meal（豆粕）, palm oil（棕榈油）, soybean oil（豆油）, PVC（聚氯乙烯）, cathode copper（铜）, aluminum（铝）, zinc（锌）, gold（黄金）, natural rubber（天然橡胶）, fuel oil（燃料油）, rebar（螺纹钢）, wire rod（线材）. Use the settlement price namely the market volume weighted strike price of the contract to calculate their return. Considering that the CPI is monthly data, to match the data frequency, we selected the settlement price at the end of each month to calculate the one-year holding period returns. In addition, due to commodity futures can be short, they have more advantages over stocks. Sample period: 01.2010 - 03.2014.

   https://www.shfe.com.cn/statements/dataview.html?paramid=delaymarket_bc

   http://www.dce.com.cn/dalianshangpin/xqsj/tjsj26/rtj/yxq/index.html
   
   **date check** 
   
               name   min_date   max_date
1        Aluminum 2011-01-01 2015-12-01  ***2009-12 数据缺失*** 
2  Cathode_Copper 2011-01-01 2015-12-01  ***2009-12 数据缺失*** 
3        Fuel_Oil 2011-03-01 2015-12-01  ***2009-12 ~ 2011-02 数据缺失*** 
4            Gold 2011-01-01 2015-10-01  ***2009-12 数据缺失*** 
5           LLDPE 2011-01-01 2015-12-01  ***2009-12 数据缺失*** 
6  Natural_Rubber 2011-01-01 2015-11-01  ***2009-12 数据缺失*** 
7        Palm_Oil 2011-01-01 2015-12-01  ***2009-12 数据缺失*** 
8             PVC 2011-01-01 2015-12-01  ***2009-12 数据缺失*** 
9           Rebar 2011-01-01 2015-12-01  ***2009-12 数据缺失*** 
10   Soybean_Meal 2011-01-01 2015-12-01  ***2009-12 数据缺失*** 
11    Soybean_Oil 2011-01-01 2015-12-01  ***2009-12 数据缺失*** 
12  Soybeans_No_1 2011-01-01 2016-05-01  ***2009-12 数据缺失*** 
13  Soybeans_No_2 2011-01-01 2015-11-01  ***2009-12 数据缺失*** 
14       Wire_Rod 2011-02-01 2015-12-01  ***2009-12 ~ 2011-01 数据缺失*** 
15    Yellow_Corn 2011-01-01 2015-11-01  ***2009-12 数据缺失*** 
16           Zinc 2011-01-01 2015-12-01  ***2009-12 数据缺失*** 

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

- font size, color (avoid red for color blindnedd friendly, use same clolr for same item among figures, etc.), table format (align, etc.), etc. 

6. Short paper using LaTeX or Jupyter/Shiny, populating it with sections, a table of contents, and the above tables and figures 

- to be determined 

7. A beamer presentation for project using LaTeX

- to be determined 

8. One interactive app (Shiny or Jupyter notebook) describing the main finding and presenting several robustness checks

- class to be taken 

9. Results are reproducible by ensuring that the coding environment is exported and concise documentation is present

- to be determined 



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


From Slack: 
some of you are asking about grading criteria; here is a guideline (somewhat overlapping with what is stated in the .README file) of what your project must have:
- a tidy folder and file structure;
- a repository on github with a history of commits by all group members; except for the fact that it contains branch 'homework' (or similar), the repository is all about your project, so please treat it as you would an actual research project of yours;
- an informative README file briefly explaining the main finding, and indicating any information needed to reproduce the findings:
- environment that can be cloned (using an environment manager such as conda, poetry or the like, or docker);
- a well maintained data management routine: the data itself is well described, and a database is organized, with upstream and ownstream functions implemented;
- a short .pdf with the findings, compiled from latex code, with figures and/or tables designed along the standards described in the lecture on visualization; the source code is uploaded;
- a .pdf with the presentation that you could use in a conference, compiled from latex code; the source code is uploaded;
- one app for the user to scrutinize the findings.


