# Web Scraping for Doctor Information
## Overview
This Python script extracts information of all the doctors in Moscow, their specializations, and their URLs from the website https://prodoctorov.ru/. Then, it navigates to the pages of each specialty and collects information of all the doctors in those specializations. Finally, it saves the information in a list of dictionaries containing the following features: 
* name
* URL
* specialization
* price
* years of experience
* category of each doctor

The final part is EDA.

The script is a part of homework for the HSE course Specialist in Data Science and is made for educational purposes only. All credits to https://prodoctorov.ru/. 

## Required Libraries
This project uses the following libraries:

* requests
* os
* numpy
* pandas
* BeautifulSoup
* selenium
* time
* random
* re
* tqdm
