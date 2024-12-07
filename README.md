# module-11-challenge

## Background
### Per BootCampSpot page:
> You’re now ready to take on a full web-scraping and data analysis project. You’ve learned to identify HTML elements on a page, identify their id and class attributes, and use this knowledge to extract information via both automated browsing with Splinter and HTML parsing with Beautiful Soup. You’ve also learned to scrape various types of information. These include HTML tables and recurring elements, like multiple news articles on a webpage.

## Assignment Breakdown
### Part 1 - Mars News
- Used Splinter library to access the Mars news website via automated browsing.
- Used BeautifulSoup to extract HTML text elements from the website.
- Used a for loop to extract article titles and preview summaries from the BeautifulSoup object. The titles and summaries are added to a dictionary, which is the appended to a list.
- Printed the completed list to confirm success of extraction.

### Part 2 - Mars Weather
- Used Splinter to access a page with a table containing Mars temperature and atmospheric pressure data.
- Stored the table into a BeautifulSoup object.
- Used a for loop to extract the rows of data into their respective variables (id, terrestrial_date, etc); the data is then added into a dictionary, which in turn is appended to a list.
- After, I converted `scrape_list` to a DataFrame. All columns were in string format so I cast appropriate data formats to speicfic columns.
- Used the DataFrame to answer the following:
    - How many months exist on Mars?
    - How many Martial days' worth of data are there?
- Data visualizations were created to answer the following questions:
    - Which month, on average, has the lowest temperature? The highest?
    - Which month, on average, has the lowest atmospheric pressure? The highest?
    - How many terrestrial days exist in a Martian year? (Rough visual estimate)
- Exported the DataFrame to a CSV file.

## Repository Breakdown:
- README.md
- .gitignore
- mars_weather_data.csv
- part_1_mars_news.ipynb
- part_2_mars_weather.ipynb