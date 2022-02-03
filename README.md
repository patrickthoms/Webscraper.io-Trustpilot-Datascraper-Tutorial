# Trustpilotscraper-Transformer 500.000 Comments scraped in 2 Days in an analyzable format

Short Description
This is a functional data web scraper method for ANY Trustpilot.com feedback/reputation site. It collects all comments and transfers them to a CSV. text document. It took me about 2 days to get 500,000 comments. Admittedly, this is a very manual method. But the main thing is that this method works and works great. 
The method consists of 2 steps. 1. The Data-Scraping-Process and 2. the CSV. Transformation process with Python. Both steps I will try to explain in detail.

Python Use:
- The Python script allows to convert some lines that are in the wrong format, like the date, which is a str and therefore not good to use for Data Science. Außerdem fügt es die Kommentare in ein übergreifendes Dokument zusammen, sodass alle einzelnen Scraping Seiten in einem Dokument hinterlegt sind. +Extra ich werde noch wenige Python funktionen ergänzen, die es euch erlauben verschiedene Daten an die Gescrapten Dokumente zu erweitern und funktionen in welchen Kommentare auf Jahre gruppiert werden können, sodass ihr Bewertungsdurchschnitte pro Jahr erhalten könnt. 


There are already some working lines in the Python script. I developed this script for my master thesis. Therefore, I have a detailed description in it. Below you can find a summary of my master thesis.

# Step 1: Data-Scraping Process - Quick Tutorial
1. Install the webscraper.io Addon to your browser. Go to https://webscraper.io/ click on install.
3. Go to your Browser (e.g. Firefox or Chrome) in which you installed the Addon and press CTRL+I+SHIFT, or do a Right Click on your Browser and select Inspect. For more Information see https://developer.chrome.com/docs/devtools/open/ (Same Function in Firefox).
4. Gehe zum Reiter Webscraper.io
5. Clicke auf "Create new Sitemap" and select "Import Sitemap"
6. Importiere die Sitemap welche ich dir im Sitemap ordner abgelegt habe. Diese ist generell. 
7. 

# Auszug aus meiner Masterarbeit


# Bugs that happend to me:
-No Scraping function on Windows 10 Chrome browser. Try Firefox in this case. 
