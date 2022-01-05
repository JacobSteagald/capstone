# Capstone_COVID_Behind_Bars

#Table of Contents

- [Motivation](#Motivation)
- [Technologies](#Technologies)
- [Problems & Hurdles](#Problems-&-Hurdles)
  * [Logistical Roadblock](#Logistical-Roadblock)
  * [Getting the Data](#Getting-the-Data)
 - [Link to the Presentation & Dashboard](#Link-to-the-Dashboard)


##Motivation

Over the last 22 months, the COVID-19 pandemic has ravaged our country. Hundreds of thousands dead, many thousand more suffering lifelong effects even if they recovered. In many ways, it has united us in fear. However, the pandemic has not effected everyone equally. COVID attacks the margins of society: disproportionately affecting the poor, individuals of color, those with pre-existing conditions, and those not able to seek medical attention. One space where many of the marginalized communities congregate is within the United States Prison System. For my Capstone I wanted to take a look at the ways in which these prison populations have been affected by the pandemic.

My journey started with an idea, which was quickly abandoned due to a lack of data reporting, to take a look at the comparison between privately run (for profit) prisons and federally and locally run prisons. Unfortunately, as I will discuss, there are no requirements for privately run prisons to report their COVID numbers to the Department of Corrections (hereafter called the DOC). This depressing fact means that my focus had to shift and so I focused in specifically on the differences in numbers across different prison funding sources. How did the numbers compare between Federal, State, and Immigration facilities and how did those numbers compare to state averages overall?

As we move through my presentation and into my dashboard, I hope that we can pick up on patterns and improve our understanding of the complicated dynamics affecting the prison population and their battle with the pandemic.

##Technologies

I wanted to demonstrate a range of skills within this project, to highlight what I had learned during my time in NSS. To do this, I focused in on ETL using Python 3 and Jupyter notebook. I pulled data from a wide range of sources, using some published data from GitHub repositories as well as webscraping data from the CDC and The COVID Prison Project to round out my numbers and gain some national context.

Once I had pulled my data in, I used Python to do my data cleaning and merging before exporting things over to Power BI to create the final Dashboard that I will be presenting. Power BI and arcGIS maps allowed me to visualize and display the data in a way that will be readily accessible and easier to understand, rather than looking at a page full of code and numbers.

##Problems and Hurdles

###Logistical Roadblock

As I mentioned in my Motivation section, one of the biggest problems I faced was the need to abandon my original idea. All prisons in the United States which receive funding from the federal or state governments are required to report COVID cases and deaths to the DOC. This allows the government to keep track on outbreaks and death rates of prisoners, as well as potential risks to guards/employees and local populations.

Unfortunately, privately run prisons do not take funding from the federal government and are therefore exempt from this requirement. As such, the numbers reported are almost assuredly an undercount and probably a dramatic one. We will dive into the numbers available to us but please understand that whatever we see is only a portion of the picture and legislation to require private reporting would go a long way to assisting this population.

###Getting the Data

In many ways, one of the most challenging aspects of this project wasn't finding the data but pulling and compiling the data in such a way that it would be useable. There are many organizations that are tracking COVID within prisons across the country. Unfortunately, much of their data is incomplete, given that they only have access to jurisdictional data or to the data in the state they reside in. In search of data I came across the Marshall Project and the UCLA School of Law. Both programs had been pulling data straight from the DOC in order to keep track of numbers. Pulling their repositories from GitHub, cleaning, and merging them together via Python I was able to compile a relatively complete look at the rates of COVID within many prison sites across the country.

I wanted to add an additional level of context, about the nation as a whole, as well as supplement the readily available data and check that the numbers I was pulling in were right. As such, I also went through a round of webscraping to pull in data from the CDC as well as the COVID Prison Project. This data bases were pulled and cleaned using Beautiful Soup, which allowed me to turn them into nice Pandas Dataframes and then export them into Power BI as I did the rest of my data.

##Link to Presentation & Dashboard

https://docs.google.com/presentation/d/1VMUeFhUzx4-4WKXiLW9Yv8auZ82fm5xZPc9j9PijVVI/edit?usp=sharing
https://app.powerbi.com/groups/me/reports/c04b6dc1-321a-40e9-911f-07f51d5bb2e9/ReportSection17b1626cbd8ea6a9aa1d
