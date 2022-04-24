# GIT-Ironhack-Data-Viz


<h1 align="center"> IBGE </h1>
<h1 align="center"> Data Gathering & Visualization </h1>



![Data_Gahering1](https://user-images.githubusercontent.com/99502330/164989944-fb18a4a0-3dfd-42b6-87bd-5bccda6e706c.jpg)



<h1 align="left"> Main Objectives </h1>

The data visualization project is an important step in the workflow of a data analyst. It helps people take decision in a data driven manner and gain insights.




<h1 align="left"> Gathering Process </h1>


![Data_Gahering4](https://user-images.githubusercontent.com/99502330/164993238-9e42eba2-012f-4e56-82b5-5e538803d11b.jpg)

<h1 align="left"> Libraries </h1>



<h1 align="left"> The Datasets </h1>

![pptB327 pptm  Autosaved](https://user-images.githubusercontent.com/99502330/164989376-bad9b7db-7280-400c-adbf-c4bcf1ea0f4c.png)

The population projections gathering in this project will support the analysis and simulations of the macroeconomic impacts.

<h2 align="left">  Population Projections for Brasil </h2>
  
Population projections for Brasil were prepared by IBGE (2010 to 2060) and IPEA (2060 to 2100). 

Data about IPEA were colleted mannually. Data available at: https://www.ipea.gov.br/portal/index.php?option=com_content&view=article&id=38577&catid=10&Itemid=9.



<h2 align="left">  World Population Projections </h2>

World population projections were prepared by ONU and The Lancet.

Data about ONU were colleted mannually. Data available at: https://news.un.org/pt/story/2019/06/1676601 and https://news.un.org/pt/story/2017/06/1589091-populacao-mundial-atingiu-76-bilhoes-de-habitantes.

Data about The Lancet were colleted mannually. Data available at: https://www.thelancet.com/journals/lancet/article/PIIS0140-6736(20)30677-2/fulltext.

This project has 2 dataframes collected from IBGE (general data and data by age group) and 2 dataframes created using IPEA information.

<h1 align="left"> ETL Process </h1>

Population projections for Brasil by IBGE (2010 to 2060) is available at: https://www.ibge.gov.br/apps/populacao/projecao/index.html?utm_source=portal&utm_medium=popclock&utm_campaign=novo_popclock. 

I used Selenium as a tool for performing web-scraping using an automated-browser. A technical problem appeared in the middle of the process of gathering but I worked around using Google Sheet to collect data.

The file had many headers inside the rows, so I collect data into the file by parts. IBGE returns one file for state and I concateneted all states into an unique dataframe. 


<h1 align="left"> Tableau Project </h1>

This project is available at: https://public.tableau.com/app/profile/patricia.ruiz/viz/Data_Viz_Project_16507585904780/BrasilXMundo?publish=yes


