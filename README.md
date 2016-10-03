# Wildfire *(Demo version)*

##Introduction
Wildfire is a tool that takes a query and processes relevant Tweets to display its sentiment distribution geographically. Through sentiment analysis, Wildfire can provide useful information regarding a given query's favorability.

This tool was created for "USC vs UCLA - Open Hack 2015" where it won 3rd place.

##Implementation
Wildfire processes relevant Tweets through a sentiment classifier which assigns to a given Tweet a positive or negative sentiment value. The Tweets are also geocoded so that their sentiment values can be displayed on a heatmap. These values are visually assigned either the colors blue (for positive sentiment) or red (for negative sentiment).

##Usage
* Enter OAuth credentials in wildfire/heatmap/confidential.py
* From project root, run `python wildfire/manage.py runserver` or `gunicorn --pythonpath wildfire wildfire.wsgi`
* Visit [localhost:8000](localhost:8000)

##In-progress
* Scaling js-img-slider to fit any screen
* Addressing utf-8 encoding issues with views.py for Heroku deployment
* Scaling Wildfire for queries beyond demo data

