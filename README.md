# Trustpilotscraper-Transformer 500.000 Comments scraped in 2 Days in an analyzable format

The method consists of 2 steps. 1. The Data-Scraping-Process and 2. the CSV. Transformation process with Python. Both steps I will try to explain in detail. 
I'm new to Github, this is my very first post/project/tutorial. If anything is not right, don't be afraid to point it out to me, preferably with a solution. If you are only interested in data scraping, then only the first step is interesting for you. 

## Webscraper.io Use:
- This is a functional data web scraper method for ANY Trustpilot.com feedback/reputation site. It collects all comments and transfers them to a CSV. text document. It took me about 2 days to get 500,000 comments. Admittedly, this is a very manual method. But the main thing is that this method works and works great.
- You can change anything you want in the web scraper. I have introduced two functions here. One is the paginator function, which automatically selects the next page and the scraper function which collects all the data for a specific comment and puts it into a row in a CSV. Document. This is the user name, the date, the rating text, the rating, the country, the comment ratings and the number of user views. 

## Python Use:
- The Python script allows conversion of some rows that are in the wrong data format, such as the date, which is a str and therefore not suitable for Data Science. It also combines the comments into one document so that all the individual scraping pages are contained in one document. 
- In addition, I'll add a couple of Python script tools that allow you to add different dates to the scraped documents, as well as functions that allow you to group the comments by year, so you can get rating averages per year.

# Step 1: Trust-Pilot Data-Scraping Process - Tutorial
1. Install the webscraper.io Addon to your browser. Go to https://webscraper.io/ click on install.
3. Go to your Browser (e.g. Firefox or Chrome) in which you installed the Addon and press CTRL+I+SHIFT, or do a Right Click on your Browser and select Inspect. For more Information see https://developer.chrome.com/docs/devtools/open/ (Same Function in Firefox).
5. Go to the tab Webscraper.io
6. Import a new sitemap. Click on "Create new Sitemap" and select "Import Sitemap". Now copy the entire content from the document "Sitemap_Trustpilot.com" stored in the Github project into the field next to the text "Sitemap JSON". Name this alternatively. In my case I name it "Example". Then click on Import Sitemap. 
7. Switch to the "Sitemaps" tab and click on the imported sitemap.
8. Set the starting point of the scaper. Just change the metadata to scrape your desired pages. Go to the tab "Sitemap [Your Sitemap Name]" in my case it is "Sitemap Example". Then select the sub-item "Edit Metadata". 
8. The starting point should have the following format "https://www.trustpilot.com/review/www.EXAMPLE.com?languages=all". This would be the example page, if I want to scrape reviews for google.com "https://www.trustpilot.com/review/www.google.com?languages=all". If you want to scrape all languages and not just be limited to English reviews, expand the Trustpilot URL with "?languages=all" here.
9. Ready, the scrapping can start. Go back to the tab "Sitemap [Your Sitemap Name]" in my case it is "Sitemap Example". You can leave the request/pageload interval as it is, it only indicates the speed of the scraper and you can change it as you like. Be careful, with high traffic it can come to timeouts/blocks from time to time. 
10. click now on Start Scraping. Unfortunately you have to scroll down again and select 1 time "next page". After that you can let everything scrape in the background. Tip: Depending on your processor power you can have several instances scrape at the same time. You only have to start the process once and always scroll down once initially and load the next page.
11. The scraper will give you a short message when the process is finished. 
12. Now export the data. Again go to the tab "Sitemap [Your Sitemap Name]" in my case it is "Sitemap Example". And select "Export data as CSV".
13. done.

# Step 2: Data processing with Python Pandas
In meinem Beispiel habe ich Anacondas verwendet. Es sei gesagt, dass es hierbei zahlreiche alternativen Möglichkeiten gibt

# Auszug aus meiner Masterarbeit
Translated with deepL.com

# Bugs that happend to me:
-No Scraping function on Windows 10 Chrome browser. Try Firefox in this case.
-Bei sehr großen Seiten mit mehr als 10.000 Kommentaren stürzt der Scraper öfters mal ab, bzw. ist instabil. Hierbei rate ich die Geschwindigkeit vor dem Scraping Prozess zu erhöhen. 
