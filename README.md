# MemePoke
![Website](https://user-images.githubusercontent.com/25799076/116272464-d49e7280-a778-11eb-83b7-37ca2a9c8dc8.png)
## Motivation
Imperial College London recently hosted the IC Hello World, a 24 hour-long hackathon targetted towards people who have never participated in a hackathon before. I lead a team with three other developers to create an app that could bring people together over long distances. We placed second in our category, and are all very proud of the project.

## Introduction
MemePoke is a web app that scrapes for the top memes of the day from Reddit, and then displays those memes to users using Reddit's CDN and allows users to vote on if they like the meme or not. The user may then find people with similar meme preferences to match with and chat live with them over the browser.

## Technology
The project was written in JavaScript, with NodeJS, ExpressJS, and Socket.io as the server technologies. The front-end was made using Semantic-UI and the database we used was MongoDB. The web application is hosted on Heroku and the database hosted on MongoDB Atlas. The memes were scraped using Java. We were one of two teams who had a fully launched application at the end of the 24 hours.

The matching algorithms works by keeping two sets for each user: the set of meme ids that they like, and the set of meme ids that they disliked. The two sets are then compared very quickly due to efficient set unions and then potential matches are ranked by the similarity of these two sets.

## Getting Started
If you want to get the project running immediately or wish to tinker around with the code, this is the place to start!

### Prerequisites
All you need is a modern browser, and go on http://memepoke.herokuapp.com/ to start using the application.
Note: as we are using the free version of heroku, the server is put to sleep after a period without use. This means that the first time using the server is slower if there aren't many users because heroku has to start it up again.

## Authors

* **Jordan Hall** - *Project Manager/Full stack developer* - [PlatinumNinja72](https://github.com/PlatinumNinja72)
* **Oliver Killane** - *Full stack developer*
* **Constantinos** - *Algorithms developer*
* **Panayotis** - *Web scraper developer*
