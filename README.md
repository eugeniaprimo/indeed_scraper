# <h1 align="center"> Indeed Scraper script with Python </h1> 

1. [Description](#1.Description)
2. [Requirements](#2.Requirements)
3. [Output](#3.Output)

## 1.Description
This scraper retrieves job openings from Indeed based on specified filters. It utilizes Selenium and iterates over the first 5 pages. Follow these instructions to run it:
1. Download the Chrome driver and install it on your computer. If there is problem running the script with the Chrome driver in the repository, check for the suitable one for you on this website: https://chromedriver.chromium.org/downloads
2. Specify the driver path and filters in the "configuration.json" file. You should modify:
   * driver_path: the path of your Chrome driver
   * keywords: job positions to filter the search
   * location: the location of the job positions. Take into account that the scraper is accessing the website of each country.
   * countries: abbreviation of the country to look for job positions on the indeed website of each country. Make sure that the URL exists if you modify this. If nothing is passed here, the scraper will recognize your location and access to the Indeed URL of that country. 

## 2.Requirements
The requirements for this scraper are specified in "requirements.txt" file. When you run the notebook, it should be installed. 

## 3.Output
The scraper saves the job positions in a csv file with the following information: 
* job_title: the title of the open job position 
* company_name: the name of the company that is looking for that job position
* location: the location of the job position
* salary: the salary, mainly on an annual basis, of the position
* url_country: the Indeed URL country that the scraper is accessing 
* extraction_date: the date when the scraper is executed
If this information is not found in the job card, the data is completed with "Not Specified".
When you execute the scraper, only the new job positions are saved in the database; it does not duplicate the job positions.

If you have any doubt, do not hesitate to contact me (lic.eugeniaprimo@gmail.com)
