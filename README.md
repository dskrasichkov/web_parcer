# Web Scraping for Doctor Information
## Overview
This project aims to extract information about doctors from prodoctorov.ru using Python.

Main features of the resulting dataset: 
* name
* URL
* specialization
* price
* years of experience
* category of each doctor

The final part is EDA.

The script is a part of homeetask for the HSE course "Specialist in Data Science - 2023" and is made for educational purposes only. All credits to https://prodoctorov.ru/. 

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

## Steps
### 1. Create a list of all large cities
The list of all large cities is extracted from the page https://prodoctorov.ru/town/ using BeautifulSoup.
The cities_links variable contains the list of links of all large cities. 
It is possible to iterate through this list, however due to CAPTCHA issues on the website I picked selenium method. 
Due to the the fact that selenium might be slow, only data from Moscow is extracted.
### 2. Get a list of links of all doctors' specialties in Moscow
The list of links of all doctors' specialties in Moscow is extracted using BeautifulSoup.
### 3. Get doctors' info from all of the pages of every specialty in Moscow
The get_doctor_info function extracts information about doctors from each page of every specialty in Moscow.
The function returns a list of dictionaries containing information about each doctor.
### 4. Iterate through every specialty
The information about doctors is extracted for every specialty in Moscow using the get_doctor_info function.
### 5. EDA
Basic statistics and analysis such as mean, median, std, outliers, slices by speciality and categoty and some vizualisation. 
