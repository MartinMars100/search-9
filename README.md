Treehouse Techdegree Project 12 - Capstone Project The app features an index page of body therapies in the North Charlotte Area. The app features an Express Server, Node.JS, Mongo DB, and Bootstrap CSS. The app will be hosted on the Heroku Site. From the index page a detail link can be clicked to see more details about the therapy. The app features a log in which authenticates through Facebook. The app features a way to add, modify and delete user and therapy data by an administrator. The Therapy List and User List (which link to edit pages) are only displayed for user's that are logged in who have admin rights set to true. Logged in users and admin users are tracked using req.session data. All log in and signup links go to facebook for facebook authentication. I don't allow for any email or user name changes. User name and email come from Facebook and are not changed. Only user admin rights can be changed. The app shows a Twitter page which shows the last 5 tweets from the Search Therapy Twitter Page. See instructions for running app below.

To Run the Site Locally
Find the App on Github and download it Run npm install to install dependencies listed in the package.json file.
Type mongod in the terminal.
Open another terminal and type mongo
Once mongod and the mongo shell are open. 
Each person who runs this locally must use their own keys which can be entered on the command line when
running the app.
It should look something like this:

FACEBOOK_APP_ID=000000 FACEBOOK_APP_SECRET=62cccc NODE_ENV=development  
TWIT_ACCESS_TOKEN=0005 
TWIT_ACCESS_TOKEN_SECRET=iiii0000  TWIT_CONSUMER_KEY=T33300
TWIT_CONSUMER_SECRET=6rrrr000   node app.js

Keep keys off github.


To run the Website in production on Heroku, put the keys
in a .env file you create from the terminal after setting up the
heroku app and adding the mongodb addon,


To Visit the Website on Heroku
Visit the Heroku Hosted Website at https://search-7.herokuapp.com/ Add therapies and use the image files to add images to display.