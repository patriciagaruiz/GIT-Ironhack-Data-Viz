# GIT-Ironhack-Data-Viz


<h1 align="center"> IBGE </h1>
<h1 align="center"> Data Gathering & Visualization </h1>

![pptB327 pptm  Autosaved](https://user-images.githubusercontent.com/99502330/164994707-b43b9598-98bc-4483-b4ed-d29d75056067.png)






<h1 align="left"> Main Objectives </h1>

The data visualization project is an important step in the workflow of a data analyst. It helps people take decision in a data driven manner and gain insights.




<h1 align="left"> Gathering Process </h1>

![Data_Gahering1](https://user-images.githubusercontent.com/99502330/164994735-d49ad9f4-b517-4ea8-a9ce-bea36561a0ad.jpg)


<h1 align="left"> Libraries </h1>

I have used in this project: selenium, pandas, requests.


<h1 align="left"> The Datasets </h1>



The population projections gathering in this project will support the analysis and simulations of the macroeconomic impacts.

<h2 align="left">  Population Projections for Brasil </h2>
  
IBGE (2010 to 2060) and IPEA (2060 to 2100) are the source of Brazilian Population projections. 

IPEA's data were mannually collected. Data available at: https://www.ipea.gov.br/portal/index.php?option=com_content&view=article&id=38577&catid=10&Itemid=9.



<h2 align="left">  World Population Projections </h2>

ONU and The Lancet are the sources of World Population projections.

ONU's data were mannually collected. Data available at: https://news.un.org/pt/story/2019/06/1676601 and https://news.un.org/pt/story/2017/06/1589091-populacao-mundial-atingiu-76-bilhoes-de-habitantes.

The Lancet's data were mannually collected. Data available at: https://www.thelancet.com/journals/lancet/article/PIIS0140-6736(20)30677-2/fulltext.

This project has 2 dataframes collected from IBGE (general data and data by age group) and 2 dataframes created using IPEA's data.

<h1 align="left"> ETL Process </h1>

Population projections for Brasil by IBGE (2010 to 2060) is available at: https://www.ibge.gov.br/apps/populacao/projecao/index.html?utm_source=portal&utm_medium=popclock&utm_campaign=novo_popclock. 

I have used Selenium as a tool for performing web-scraping using an automated-browser. I have faced a technical issue while running the gathering process, then I have worked around it using Google Sheet in order to collect the data.

These files have many headers inside the rows, so I collected the data of each file in pieces. IBGE's data returns one file for state, so I concatenated all states into an unique dataframe. 


<h1 align="left"> Tableau Project </h1>

This project is available at: https://public.tableau.com/app/profile/patricia.ruiz/viz/Data_Viz_Project_16507585904780/BrasilXMundo?publish=yes


