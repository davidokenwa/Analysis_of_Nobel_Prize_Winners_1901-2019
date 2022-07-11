# **Analysis of Nobel Prize Winners Since 1901**

> Everyone knows the Nobel Prize is one of the most prestigious awards anyone can receive. But do you know how it started? Read the article on Medium [here](https://davidokenwa.medium.com/analysis-of-nobel-prize-winners-since-1901-6838e5b2b6fd) 

| ![Nobel medal](https://github.com/davidokenwa/Analysis_of_Nobel_Prize_Winners_1901-2019/blob/main/nobel_medal.png) | 
|:------------------------------------------------------------------------------------------------------------------:| 
| **The Nobel Prize Medal**                                                                                          |

In May 2022, I joined the Onyx, Novypro and Astrato data challenge. We were asked to visualize the Nobel Prize winners 
since 1901. This was a very interesting dataset to work on as I learned so much about the Nobel Prize, learnt different 
data cleaning techniques in Excel, practiced different data exploration methods  and completed the visualization within 
a day! This is my record time for building a dashboard for a data challenge.

The Nobel Prize is an annual award given for outstanding contributions to chemistry, physics, literature, medicine, 
peace and economics. In a will drafted by Alfred Nobel in 1895 before his death, he apportioned a major part of his 
wealth to award those who in the preceding year, “shall have conferred the greatest benefit on mankind.” The prizes 
established by his will are in the fields of Physics, Chemistry, Medicine, Literature and Peace. In 1901, the first 
prizes were awarded and in 1938, the Bank of Sweden introduced a prize in Economics. Nobel Award recipients are called 
Nobel Laureates. You can read more about the Nobel Prize [here](https://www.britannica.com/topic/Nobel-Prize)

## **Background and Dataset**
The challenge required me to visualize the Nobel Prize data from 1901
to 2019. The dataset is a CSV file with 923 entries, one for each 
Laureate.

|  ![raw data](https://github.com/davidokenwa/Analysis_of_Nobel_Prize_Winners_1901-2019/blob/main/raw_data_snippet.png)  | 
|:----------------------------------------------------------------------------------------------------------------------:| 
|                                                **Snippet of Raw Data**                                                 |

I decided to tell a unique story of how we can be inspired by the 
Nobel Laureates. In fact, I gave my dashboard the sub-theme, “Let 
the Laureates Inspire You”. I wanted to explore what we can learn 
from the laureates in terms of collaboration, women's representation,
breaking invisible limitations, starting early, blooming later and
demonstrating grit and tenacity in the face of adversity. 
The laureate’s data was the perfect one to demonstrate all these 
and more!

## **Project Steps**

To arrive at the dashboard, I followed the steps outlined below:
1. Preliminary research
2. Data cleaning
3. Data exploration
4. Data Visualization
5. Insight

|  ![project steps](https://github.com/davidokenwa/Analysis_of_Nobel_Prize_Winners_1901-2019/blob/main/project_steps.png)  | 
|:------------------------------------------------------------------------------------------------------------------------:| 
|               **Project Steps. Onyx Nobel Laureates Challenge.** _Designed by David Okenwa in PowerPoint_                |

### **1. Preliminary Research**

I did some research on the Nobel Prize to understand what it is all about before going into the data. Taking out some 
time to brush up on the particular industry or subject your data analysis is based on will make your analysis a lot 
more effective. You will know what to expect and know when things are veering off normal or when the data is unreliable.
During my preliminary research, I also got some colours associated with the Nobel prize and generated a palette using 
[Coolors](https://coolors.co/). The colour palette influenced my choice of colours for my final dashboard.

|  ![colour palette](https://github.com/davidokenwa/Analysis_of_Nobel_Prize_Winners_1901-2019/blob/main/coolors.com.png)  | 
|:-----------------------------------------------------------------------------------------------------------------------:| 
|                                      **Colour Palette. Generated from coolors.co**                                      |

### **2. Data Cleaning**
I loved this step because the data needed some cleaning to be 
ready for analysis. I practiced the data cleaning techniques 
I had learned and learnt new ones as I searched bottlenecks on Google.

I joined the last and first name columns to get the full names. 
The enabled me to identify laureates that received more than one 
award. I remapped inconsistent categories in countries to the same 
category name. For example, I change all “USSR (Now Russia)” to “Russia”.

Also, the countries of birth and death were given in two-letter 
country codes while the countries of university were given in full. 
I had to make all of them in the same format—codes. I converted the 
countries of university to codes. To achieve this, I imported a 
table outlining countries and their codes from [IBAN](https://www.iban.com/country-codes)
using Power Query. I then used VLOOKUP to match the countries of 
university and their codes. 

To get the number of awards given (which was less than the number
of laureates awarded), I converted the ‘share’ of awards each 
laureate had to fractions and summed them up. To get the number 
of awards given in each field, I used the conditional sum ‘SUMIF’.

| ![cleaned data](https://github.com/davidokenwa/Analysis_of_Nobel_Prize_Winners_1901-2019/blob/main/cleaned_data.png)  | 
|:---------------------------------------------------------------------------------------------------------------------:| 
|                                                   **Cleaned Data**                                                    |



### **3. Data exploration**

I explored the data to find out trends in the data for myself. I 
made extensive use of VLOOKUP and other Excel functions here such 
as SUM, AVERAGE, MEDIAN, COUNTA, COUNTIF, COUNTIFS, SUMIF, SUMIFS, 
AVEREAGEIF etc. I named columns and tables using Name Manager for 
easy access later. I made many subtables and made extensive use of 
charts. I drilled into the data to find insights based on my domain
knowledge (from preliminary studies) and more!.

Here are some of the insights I got during my exploration:

Five hundred and seventy-five prizes were presented to 923 
laureates from 73 countries. The laureates are a rare few–0.0000001% 
of the world’s population as of 2019.

| ![top highlights](https://github.com/davidokenwa/Analysis_of_Nobel_Prize_Winners_1901-2019/blob/main/top_overview_numbers.png)  | 
|:-------------------------------------------------------------------------------------------------------------------------------:| 
|                                                        **Top Overview**                                                         |

There are more laureates than prizes given because inventions by teams can win a prize.
Collaboration definitely makes the world better!

|  ![collaboration](https://github.com/davidokenwa/Analysis_of_Nobel_Prize_Winners_1901-2019/blob/main/collaborations_chart.png)  | 
|:-------------------------------------------------------------------------------------------------------------------------------:| 
|                                      **Number of Laureates and Prizes vs Field of Award**                                       |

Only 6% of laureates are women. There has however been an increase 
in the number of female laureates in recent decades, reaching 12% 
in 2010-2019

|  ![women rep](https://github.com/davidokenwa/Analysis_of_Nobel_Prize_Winners_1901-2019/blob/main/women_representation.png)  | 
|:---------------------------------------------------------------------------------------------------------------------------:| 
|                                          **Women Representation in Nobel Prizes**                                           |

56% of Laureates are from the USA, UK, Denmark or France. At least
60% schooled in those countries as well. At least 23% of laureates
were international students.

| ![countries](https://github.com/davidokenwa/Analysis_of_Nobel_Prize_Winners_1901-2019/blob/main/countries_of_laureates.png)  | 
|:----------------------------------------------------------------------------------------------------------------------------:| 
|                                    **Countries of Laureates and Countries they Schooled**                                    |

I then went ahead to highlight four laureates whose stories were
inspirational. They are Marie Curie, Malala Yousafzai, John Goodenough and Josh Nash.

| ![most inspiring](https://github.com/davidokenwa/Analysis_of_Nobel_Prize_Winners_1901-2019/blob/main/inspirational_laureates.png)  | 
|:----------------------------------------------------------------------------------------------------------------------------------:| 
|                                                    **Most Inspiring Laureates**                                                    |

### **4. Data visualization**

After exploration, I had the task of putting them together in one piece. After a lot of experimentations and 
rearrangements and alignment and formatting, I came up with the dashboard below. I gave the background a nice paperlike 
feel and removed all unimportant and distracting information from the charts.

| ![dashboard](https://github.com/davidokenwa/Analysis_of_Nobel_Prize_Winners_1901-2019/blob/main/000Dashboard_FULL.png)  | 
|:-----------------------------------------------------------------------------------------------------------------------:| 
|                     **Onyx Nobel Prize Dashboard** _Designed by David Okenwa with Microsoft Excel_                      |

### **5. Insights**

The insights were stated during the analysis. Here is the highlight:
* Many prizes were won by teams through collaboration. Collaboration makes the world better. In the word of Helen Keller,  "Alone we can do so little; together we can do so much."
* Women's representation in the Nobel prize is rising in the current century.
* Most laureates are from or schooled at USA, UK, France and Denmark.
* It's not too early to stand out and never too late to blossom.

---

### **Relevant Links**

Thank you for reading up to this point! Here are some relevant links:

* [Medium article](https://davidokenwa.medium.com/analysis-of-nobel-prize-winners-since-1901-6838e5b2b6fd)
* [LinkedIn Post](https://www.linkedin.com/posts/david-okenwa_david-okenwa-onyx-nobel-prize-data-challenge-activity-6936211331779805184-7q0O?utm_source=linkedin_share&utm_medium=member_desktop_web)
* [Dataset](https://www.kaggle.com/datasets/bahramjannesarr/nobel-prize-from-1901-till-2020)
