# Scraping_python_profiles_from_GitHub

 This code scrapes trending python developers, their popular repo details from [https://github.com/trending/developers/python?since=daily](https://github.com/trending/developers/python?since=daily). Navigates to each profile pages and grabs required details. The information collected is exported to a csv file.

## Motivation
* The main idea behind writing this set of web-scraper code, was to gain insights from top Python developers profile and their popular repositories on GitHub.
* I was curious to know about the owners and contributors of the trending repositories who I presume are experts or competent in Python and worth following.
* Thus, I decided to extract the profiles of these users to gain some interesting insights into their background.

## Web Scraping
Web Scraping is the process of parsing and extracting data from websites. It is a useful technique when we want to collect data from websites for our work.

## Tools used for Web Scraping
* Programming Language: Python

Python Libraries: 
1. Requests - To download the web page,to fetch the data from the URL
2. BeautifulSoup - to parse the HTML content
3. Pandas - to create dataframe

## Steps involved 
* Accessing the HTML content of the webpage using requests:

  Website used for scraping [https://github.com/trending/developers/python?since=daily](https://github.com/trending/developers/python?since=daily)
* Parsing the HTML content using beautiful soup
* Extracting the required data by navigating through the parsed tree.
     * From the trending page, Scrape the Developer name, profile URL, popular repo, repo URL, repo description.
     * Navigate to the Profile page. Scrape the following details:
          * Bio
          * Company
          * Location
          * Total contributions this year.
     * Store the extracted information to a DataFrame.
     * Finally, export the DataFrame to a csv file.




