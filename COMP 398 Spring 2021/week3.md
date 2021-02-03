# Week 3

## Monday
- Daniel seems like a competent guy. I hope that he turns out to be a good programmer. This is his first time working with the librairies that I am using so I'll limit my expectations for this week.
- I have made some work on the libraries of the backend.
    - Now have an accessor method to make a BeautifulSoup object out of any page from Congress.gov
    - I have cloned the code from the Metrics Dashboard databaseConnector.py file into the project to simplify the storing of data.
- Looking at the Congress.gov search feature, there is an option to save the first 1000 responses of a search.
    - I do not think that this will help in my research.
        - While useful, the data will need to be converted into a .db file anyway

## Tuesday
- I cranked through the Member Collector on a caffine fueled diet
- The code is working, however it is only getting member front matter. In order to go deeper, I would neeed to scrape BioGuide or all of the bills associated with a member
    - Since I am already scraping bill information, it would just make more sense to make that into its own module IMO
    - All that is left to do is to Dockerize it, make sure that it scrapes both the House and Senate, implement argparse, and implement whiptail

## Wednesday
- I bug fixed the code today, it seems to work well enough to call it quits on that
- I still have to implement the Docker container, and ensure that it is scraping both the house and senate, as well as the argparse and whiptail features
    - Might be a good idea to prevent the other modules from being ran automatically
- Still need tests to be written for a few of the modules
    - Will have to learn how to use GitHub Actions for CI
