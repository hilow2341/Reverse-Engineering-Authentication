Unit 14 Sequelize Homework: Reverse Engineering Code
-APP DESCRIPTION-
This app enables it’s users to create an account, log into their account and sign back out. The data created by the user is subsequently stored in the backend with a mysql database.

-USER STORY-
AS A user who wants to securely create an account,
I WANT to know my personal details are safely stored,
SO THAT I can feel confident about utilizing this website.

-NODE MODULES USED-
Express, mysql2, Passport, bcrypt, Sequelize

-INSTALLATION-
1.Create a mysql database such as “passport_demo”
2.In config.js, fill in personal information
3.Within your repository open the terminal and run “npm i” to install the node packages
4.Also in the terminal, run “node server.js” to connect to your server
5.Open your browser and local host to run the app

-FILES EXPLANATION-

config/middleware: 
“isAuthenticated.js”
-Restricts routes that the user isn’t allowed to have access to. Subsequently, if the user is logged in, the request to the route is accepted.

config/
“config.json”
-Configuration to connect to a server.
“passport.js”
-Javascript which enables users to log in with an email and password.

models/
“index.js”
-Connects to a database and imports user login data.
“user,js”
-File defines what is stored in the database as well as using bcrypt to make our database information securely stored.
public/
-Stores front end html and equivalent javascript functionality. It also contains css styling.

routes/
“api-routes.js”
-Includes routes for signing in, logging out and getting user specific data to display client side.
“html-routes.js”
-Routes that check whether a user is signed in or if the user already has an account, and sends them to the correct html page.

Parent Files:
“package.json”
-Contains all package info, node modules used, version info, etc…
“server.js”
-Requires packages, sets up PORT, creates express and middleware, creates routes and syncs database / logs messages within the terminal on a successful connection to your server.

CHANGES:
Changes can be made with the type of database you want to use. Important changes could include different packages used for keeping your information secure. Other changes could be the appearance and functionality of the front end.
