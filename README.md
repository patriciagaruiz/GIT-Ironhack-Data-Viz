# GIT-Ironhack-Data-Viz


<h1 align="center"> IBGE </h1>
<h1 align="center"> Data Gathering & Visualization </h1>

![pptB327 pptm  Autosaved](https://user-images.githubusercontent.com/99502330/164989376-bad9b7db-7280-400c-adbf-c4bcf1ea0f4c.png)




<h1 align="left"> Main Objectives </h1>

The data visualization project is an important step in the workflow of a data analyst. It helps people take decision in a data driven manner and gain insights.

![Humans are friends!](https://user-images.githubusercontent.com/99502330/161834340-92521684-877f-495d-8df9-ec22bfacb2fc.jpg)


<h1 align="left"> Gathering Process </h1>


<h1 align="left"> The Datasets </h1>

The mission of the Global Shark Attack File is to provide current and historical data on shark/human interactions for those who seek accurate and meaningful information and verifiable references.
Dataset available at: https://www.kaggle.com/datasets/teajay/global-shark-attacks.


<h1 align="left"> Import File </h1>

The dataset has 25.723 lines and 24 columns.

<h1 align="left"> Heatmap before dropping duplicate values and empty columns </h1>

![Heatmap_before](https://user-images.githubusercontent.com/99502330/161841837-245a2a81-1254-468b-85cd-5caeb78c776a.png)

<h1 align="left"> Heatmap after dropping duplicate values and empty columns </h1>

![Heatmap_after](https://user-images.githubusercontent.com/99502330/161843475-aaa14977-13fe-4672-b22b-6c18c98d915e.png)


Cleanned Dataset has 6.302 lines and 23 columns.

<h1 align="left"> Libraries </h1>

I used in this analysis: pandas, numpy, re, seaborn, pandas_profiling.

<h1 align="left"> 1. Are there more fatal than non-fatal attacks? </h1>

This answer needs a clean column called: Fatal (Y/N).
First of all, I used 'groupby' to discover the number of lines per value. Here the results: 2017, N, M, Y, y, UNKOWN.
I read the lines with values different from Y or N and changed (with mask and loc) the wrong values by Y, N or X (for unclear cases where the identification was not possible).

CONCLUSION: There are more non-fatal attacks according to the data.

Total Shark Attacks with Known Results: 5692 attacks

Fatal Shark Attacks: 1389 attacks / 24.4 %

Non Fatal Shark Attacks: 4303 attacks / 75.6 %

*** Attacks with Unknown Results: 71 attacks / 1.23 % (disregarded in the previous analysis)

![shaaark183](https://user-images.githubusercontent.com/99502330/161834643-751fe82d-f9d7-4b89-8836-52da63639d59.jpg)




<h1 align="left"> 2. Are there more attacks for male or female? </h1>

This answer needs a clean column called: Sex.
First of all, I used 'groupby' to discover the number of lines per value. Here the results: . , F, M, N, lli.
I read the lines with values different from M or F and changed (with mask and loc) the wrong values by M, F or X (for unclear cases where the identification was not possible).

CONCLUSION: There are more attacks to male according to the data.


Total Shark Attacks with Known Gender: 5735

Male Shark Attacks: 5098 attacks / 88.89 %

Female Shark Attacks: 637 attacks / 11.11 %

*** Attacks with Unknown Results: 71 attacks / 1.23 % (disregarded in the previous analysis)




![shark_boat_men](https://user-images.githubusercontent.com/99502330/161890970-fcc257d9-9f09-42db-b784-7946a1875867.gif)











<h2 align="left"> OTHERS CONCLUSIONS </h2>
Crossing valid lines related to fatal attacks (5.692) and attacks by gender (5.735) I extracted a double groupby:


![Graf2](https://user-images.githubusercontent.com/99502330/161976678-71fc281b-da1f-4baf-a9a8-c34394f00f42.png)


<h1 align="left"> 3. Are shark attacks influenced by hemisphere? </h1>

This answer needs a clean column from main database called: Country.
Even though this column does not provide the information needed to answer the question because it doesn’t tell in which hemisphere the country is, I used a database of coordinates (latitude/longitude) to find out this information. I used a database of coordinates (latitude/longitude) for countries to find out this information. Dataset available at: https://www.kaggle.com/datasets/max-mind/world-cities-database.

![sharks-swimming](https://user-images.githubusercontent.com/99502330/161890934-c355c48d-616a-4ac3-aa84-67fa93ead0bc.gif)

I used 'unique' to discover the values into the main database (199 countries) and compared (merge) with the database of coordinates. I used 'mask' and 'loc'to update wrong values.
Countries after cleanning database: 141 

CONCLUSION: There are more shark attacks in Northern Hemisphere

Total Shark Attacks with Known Hemisphere: 6206 attacks

Hemisphere Northern: 3432 attacks / 55.3 %

Hemisphere Southern: 2774 attacks / 44.7 %

*** Attacks with Unknown Hemisphere: 96 attacks / 1.52 % (not inside the previous analise)



![Graf4](https://user-images.githubusercontent.com/99502330/161987256-44dd2891-dba5-4f7c-b23c-7ff58841f4a2.png)





