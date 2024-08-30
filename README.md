# Drug Count Overview
This project aims to create an interactive dashboard for the user to visualize drug available in Canada based on the ATC code, which indicates the active mechanism of the drug through time (1904-2024). 

## Data collection
Four datasets were collected from [Drug Product Database (DPD) - Health Canada](https://health-products.canada.ca/api/documentation/dpd-documentation-en.html#a2). One more dataset was scraped from [ATC/DDD Index - Norwegian Institute orf Public Health](https://atcddd.fhi.no/atc_ddd_index/) to provide more detailed information related to active therapeutic chemicals of the drug. To check the definition of certain terminology, please visit [DPD Terminology - Health Canada](https://www.canada.ca/en/health-canada/services/drugs-health-products/drug-products/drug-product-database/terminology.html).

Each dataset was cleaned and prepared so that the drugs in the finald datasets:
1. is for human
2. is not natural health products
3. has a valid atc code

Drugs with same brand name, same active compounds but not the same drug code were treated as two different drugs considering the variation of formulation and/or concentration may impact the drug schedule or drug status. 

Finally, all datasets are merged to make the `Drug Final.csv` which was used to make the final delivery. 

## Dashboard
The dashboard with interactive component was created using Tableau. Four pages were made, each contains a method to go back or forward one page:
1. Cover page: title and summary of this project
2. Dashboard 1: lineplot of number of new drugs on market each year, from 1904 to 2024
3. Dashboard 2: drug distribution by schedule (prescription vs OTC), drug distribution by atc (first level), drug distribution by drugs status (Currently Marketed, Cancelled Post Market, Under Review)
4. Dashboard 3: drug distribution by schedule (prescription vs OTC), drug distribution by atc (second level), top 8 companies in bar chart

The dashboard can be visited here: [Drug Count Overview Final](https://public.tableau.com/app/profile/yelin.han/viz/Test_17248809112530/D1).

---

# Overview of file attached
Four files are attached to this respositoire related to the project.

1. Drug Final: It is the final dataset in csv used to create the final dashboard
2. Drug Collection and Cleaning: It is a Jupyter Notebook file that contains detailed steps during data collection and data cleaning. It recorded all the manipulation and decision taken to reach the final dataset from the five original datasets. 
3. Presentation: It is a PowerPoint Slides that explains the structure of this project as well as the functionailites in the dashboard. 
4. Proposal: It is a docx file that contains the original proposal of this project. Although it is not strictly followed due to some technical difficulties in the process of the project, it provided a very good guideline to the project. 



