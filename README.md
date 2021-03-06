# Friend-Finder
`Go check it out :  `   https://friend-finder-appp.herokuapp.com/
## Overview
This is a compatibility-based "FriendFinder" application -- basically a dating app. This full-stack site will take in results from your users' surveys, then compare their answers with those from other users. The app will then display the name and picture of the user with the best overall match. 


### Instructions

1. There are 10 survey questions of your choosing. Each answer should be on a scale of 1 to 5 based on how much the user agrees or disagrees with a    
   question.
2. `server.js` file require the basic npm packages we've used in class: express and path.
3. `htmlRoutes.js` file include two routes:
 - A GET Route to /survey which should display the survey page.
 - A default, catch-all route that leads to home.html which displays the home page.

4. `apiRoutes.js` file contain two routes:
 - A GET route with the url /api/friends. This will be used to display a JSON of all possible friends.
 - A POST routes /api/friends. This will be used to handle incoming survey results. This route will also be used to handle the compatibility logic.

5. Save the application's data inside of app/data/friends.js as an array of objects. Each of these objects should roughly follow the format below.
  {
  "name":"Ahmed",
  "photo":"https://media.licdn.com/mpr/mpr/shrinknp_400_400/p/6/005/064/1bd/3435aa3.jpg",
  "scores":[
      5,
      1,
      4,
      4,
      5,
      1,
      2,
      5,
      4,
      1
    ]
}

6. Determine the user's most compatible friend using the following as a guide:
- Convert each user's results into a simple array of numbers (ex: [5, 1, 4, 4, 5, 1, 2, 5, 4, 1]).
- With that done, compare the difference between current user's scores against those from other users, question by question. Add up the differences to calculate   the totalDifference.
- Remember to use the absolute value of the differences. Put another way: no negative solutions! the app should calculate both 5-3 and 3-5 as 2, and so on.
- The closest match will be the user with the least amount of difference.

7. Once you've found the current user's most compatible friend, display the result as a modal pop-up.
- The modal should display both the name and picture of the closest match.

### Tools/Languages Used:
 - HTML
 - CSS/Bootstrap
 - Javascript
 - jQuery
 - NodeJS
 - Express
 - JSON
 - Heroku
 - Postman

### NPM Packages:
- <a href="https://www.npmjs.com/package/express">Express</a>
- <a href="https://www.npmjs.com/package/body-parser">Body Parser</a>
- <a target="_blank" rel="nofollow" href="https://www.npmjs.com/package/path">Path</a>

### Authors
  - Kanyarut Pornamnuay
  <br><a target="_blank" rel="nofollow" href="https://github.com/benbaba2525">Visit My Github Profile</a>
  <br><a target="_blank" rel="nofollow" href="https://www.kanyarut.me/">Visit My Portfolio</a>


### Acknowledgments
  - UCLA Coding Bootcamp   <a target="_blank" rel="nofollow" href="https://bootcamp.uclaextension.edu/coding/">Visit UCLA Coding Bootcamp</a>

### Helpful Link

  - <a target="_blank" rel="nofollow" href="https://expressjs.com/">Express.js</a>
  - <a target="_blank" rel="nofollow" href="https://www.postman.com/">Postman</a>
  - <a target="_blank" rel="nofollow" href="https://devcenter.heroku.com/articles/getting-started-with-nodejs#set-up">Heroku</a>

