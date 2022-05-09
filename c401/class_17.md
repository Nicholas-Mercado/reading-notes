# Web Scraping

## Web Scrape with Python in 4 minutes

web scraping is a automatic process of extracting large amounts of data for a website

## Before web scraping

- Read the sites Terms and Conditions
- Do not download data to fast

## useful libraries for scraping

- requests
- urllib.requests
- time
- bs4 import BeautifulSoup

## How to scrape websites without getting blocked

 Rules to be a good scraper

- Be nice and respect the robot.txt
- make your scraper slow, don't slam server
- imitate human behaviors

### ways to give away you are scraping

- scrapping to fast
- following the same pattern
- making to many requests
- Not identifing as popular browser
  - use User-Agent
- using User-Agent of old browser

### Honey pot traps

ways to detect honey pot

- link has proper visibility with no nofollow tag
- CSS style will have a display:none
