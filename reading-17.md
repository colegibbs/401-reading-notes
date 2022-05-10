# Reading 17

## [Web Scrape with Python in 4 minutes](https://towardsdatascience.com/how-to-web-scrape-with-python-in-4-minutes-bc49186a8460)

- automatically accces and extract info from a site
- saves time and effort
- each file is a .txt file and there are hundreds of them
- important notes:
  - read through the sites terms and conditions to understand how you can legally use the data
  - make sure you are not downloading datat too fast because it can break the website and get you blocked
- find where the relavent html tags are
- do this by using dev tools
- libaries to import:

```python
import requests
import urllib.request
import time
from bs4 import BeautifulSoup

#website url
url = 'siteURL'
# use beautfiulSoup to make the data structure nicer
soup = BeautfiulSoup(response.text, "html.parser")
#find all <a> tags
soup.findAll('a')
#grab relevant files and hrefs
one_a_tag = soup.findAll('a')[38]
link = one_a_tag['href']
#define dowloadable url
download_url = 'base' + link
#pause for a second to not spam
time.sleep(1)
# To download the whole data set, let's do a for loop through all a tags
line_count = 1 #variable to track what line you are on
for one_a_tag in soup.findAll('a'):  #'a' tags are for links
    if line_count >= 36: #code for text files starts at line 36
        link = one_a_tag['href']
        download_url = 'http://web.mta.info/developers/'+ link
        urllib.request.urlretrieve(download_url,'./'+link[link.find('/turnstile_')+1:]) 
        time.sleep(1) #pause the code for a sec
    #add 1 for next line
    line_count +=1
```

## [What is Web Scraping?](https://en.wikipedia.org/wiki/Web_scraping)

- extracting data from sites
- usually an automated process like a bot or web crawler
- ability to find files and save relevant data
- has many uses
- special tools and software have been made to make scraping easier
- newer scraping involves monitoring data feeds from servers, usually by intercepting json
- some site disable bots and crawlers and some bots and crawlers will capture stills of the webisite and crawl over that
- techniques
  - human copy and paste
  - text pattern matching
  - HTTP programming
  - HTML parsing
  - DOM parsing
  - Vertical aggregation
  - Semantic annotation recognizing
  - Computer vision web-page analysis

## [How to scrape websites without getting blocked](https://www.scrapehero.com/how-to-prevent-getting-blacklisted-while-scraping/)

- web crawlers are faster at getting data
- crawlers can affec the performance of the site so some site managers try to block them
- basic rule: be nice
- respect robots.txt
  - best practices
  - what will give a crawler away
    - too fast over to many pages
    - pattern
    - too many requests
    - not popular browser
- make the crowling slower, do not slam the server, treat websites nicely
- Do not follow the same crawlin pattern
- make requests through proxies and rotate them as needed
- Rotate user agents and corresponding HTTP request headers between requests
- Use a headless browser like puppeteer, Selenium or playwright
- Beware of honey pot traps
- check if website is changing layouts
- avoid scraping data behind a login
- Use captcha solving services
- How can websites detect and block web scraping
- How do you find out if a website has blocked or banned you?
  - CAPTCHA
  - unusual content dilivery delays
  - frequent response with http 404, 301, or 50x errors

## [Track Amazon Prices](https://www.youtube.com/watch?v=Bg9r_yLk7VY)

```python
#pip install requests bs4
import requests #access url
from bs4 import BeautifulSoup
import smtplib #mail protocal
import time

URL = "someUrl" #scrapping website

headers = {"User-Agent": "info about browser}

page = requests.get(URL, headers = headers)

soup = BeautifulSoup(page.content, 'html.parser')

title = soup.find(id="productTitle").get_text()
price = soup.find(id="priceblock_outprice").get_text()
converted_price = float(price[0:5])

if(converted_price < 1.700>):
  send_mail()

def send_mail():
  server = smtplib.SMTP('smtp.gmail.com', 587)
  server.ehlo()
  server.starttls()
  server.ehlo()

  server.login('gmail', 'passowrd')

  subject = 'Price fell down"
  body = "check link: URL"
  msg = f"Subject: {subject} {body}"
  server.sendemail(
    'from email',
    'to email',
    msg
  )
  print('email sent')
  server.quit()

  while True:
    check_price()
    time.sleep(60)#number of seconds to wait before running
```

## Bookmarks

- [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/)
