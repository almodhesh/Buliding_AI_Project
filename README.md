# Buliding_AI_Project
Buliding AI Project
<!-- This is the markdown template for the final project of the Building AI course, 
created by Reaktor Innovations and University of Helsinki. 
Copy the template, paste it to your GitHub README and edit! -->

# Building AI weather Recommender

this project to build can guide you if you wish to travel within dates is the weather will be good or no 

## Summary

this project to build can guide you if you wish to travel within dates is the weather will be good or no 


## Background

Must of non traveller facing challenge some times regarding to the weather when they travel. the idea is select with thim the best time during to expected weather 

This is how you make a list, if you need one:
* weather update
* recommended time 



## How is it used?

Describe the process of using the solution. In what kind situations is the solution needed (environment, time, etc.)? Who are the users, what kinds of needs should be taken into account?

Images will make your README look nice!
Once you upload an image to your repository, you can link link to it like this (replace the URL with file path, if you've uploaded an image to Github.)
![Cat](https://upload.wikimedia.org/wikipedia/commons/d/db/Nor%27easter_1967-03-22_weather_map.jpg)



   # write your solution here

import requests
from pprint import pprint

API_KEY = 'dd7200192b6c2340d7a7323ee44f87ca'   # to get this key you must register to openweathermap.org
city = input("Enter a city: ")                 # ask user to enter the city name

base_url = "http://api.openweathermap.org/data/2.5/weather?appid="+API_KEY+"&q="+city # the reqest will send to this link
weather_date = requests.get(base_url).json()    # get the result 
pprint(weather_date)   # to print the result 


## Data sources and AI methods
Where does your data come from? Do you collect it yourself or do you use data collected by someone else?
If you need to use links, here's an example:
[Twitter API](https://developer.twitter.com/en/docs)

| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |

## Challenges

What does your project _not_ solve? Which limitations and ethical considerations should be taken into account when deploying a solution like this?

## What next?

How could your project grow and become something even more? What kind of skills, what kind of assistance would you  need to move on? 


## Acknowledgments

* list here the sources of inspiration 
* do not use code, images, data etc. from others without permission
* when you have permission to use other people's materials, always mention the original creator and the open source / Creative Commons licence they've used
  <br>For example: [Sleeping Cat on Her Back by Umberto Salvagnin](https://commons.wikimedia.org/wiki/File:Sleeping_cat_on_her_back.jpg#filelinks) / [CC BY 2.0](https://creativecommons.org/licenses/by/2.0)
* etc
