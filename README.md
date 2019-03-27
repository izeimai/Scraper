# Scraper

Deployed on heroku:
https://morning-sierra-48356.herokuapp.com/

Scrapes sciencemag.com website and stores articles in Mongo database using node packages (express, mongoose, cheerio, and axios)

What does this app do? 
When the user visits the website, the scraper will scrape news stories from https://www.sciencemag.org/news/scienceinsider then displays and stores information of the scraped articles. Each article's headline, summary and URL are stored in the Mongo database. Additionally, each user can leave comments on the articles displayed that are stored in the database and can be viewed again. These comments are associated with the article so all users can see the stored comments and can also be deleted.
This app is deployed on Heroku with mLab, whoch is remote MongoDB database that Heroku supports natively.

Technologies used:
* Axios = promised-based http library (works similarly to AJAX calls) on both server and client side
* Cheerio = Package to enable server-side jQuery syntax
* Express = Node.js web application framework that handles server and routing
* MongoDB = NonSQL database to store article information
* Mongoose = ORM for Mongo database in Node.js

How is this app useful? 
Learned how to use noSQL databases like MongoDB through storing JSON objects and information as fields. It was also important to realize that given the flexibility of the MongoDB, there needs to be forms of validations in place so that no unintentional fields are created.

Future directions: 
I'd like to attempt scraping a webpage that is dynamic (used JS files to populate page) which would be more challenging. 