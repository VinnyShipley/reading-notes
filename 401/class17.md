# Web Scraping

## Definition

Web Scraping is a technique to automatically access and extract large amounts of information from a website.

## Important Notes on Web Scraping

* Read through the terms and conditions to understand how to legally use a set of data when scraping.

* Make sure you don't download data too fast and break the website. This can result in you being blocked from the website.

* Involves a fetching and an extraction phase. Fetching is the downloading of a page, and the extraction is the parsing of that information and formatting it to a usable amd readable condition.

## Steps to Scraping

* Figure out how to access the relevant data within the website. This can be done by targeting specific HTML tags on the site

* For Python, import the following libraries:

      import requests
      import urllib.request
      import time
      from bs4 import BeautifulSoup

* Set a variable called url to the the website, and then access the library with the request library

* If successful, you should get a 200 response

* Next, use BeautifulSoup to parse through the response data. Docs for BeautifulSoup can be found [here](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)

* Use the .findall method to find all of your created \<a> tags.

* Finally convert the information contained at the end of the link into a .txt file and save it to your computer

## How to Scrape Websites without being blocked

[Reference Reading](https://www.scrapehero.com/how-to-prevent-getting-blacklisted-while-scraping/)

* The over arching rule of scraping (and honestly life. It's the not that complicated people), is to 'Be Nice'. Follow a websites crawling policies.

* Respecting the robot.txt file is important when considering scraping a website. if it contains the lines

      User-agent: *

  or

      Disallow:/

  it means that the site does not want to be scraped.

* Make the crawling slower and do not slam the server. This means slowing down your scraper so the website is not put under unneeded stress from the scraping and crawling of the site. When creating a spider to traverse the page, put in some elements to suggest that it is fact not a program. This will both slow down the traversal as well as make it look more human in nature

* Change your IP address as needed so it isn't apparent you are a scraper

## Things I want to know more about

* The converting into text files and then using that information is still a little confusing to me.

* It's not explicitly stated, but it sounds like you can only scrape information that is found in a link from the page you are trying to scrape from?
