# Blogbook: A Full Stack Online Blogging Platform

## Exciting Features

* Authentication
  * Login using Username and Password
  * Google Authentication
* CRUD - Create, View, Edit and Delete Articles

## How to Run this app?

* Install and start MongoDB server locally (or online), and get `MONGODB_URL`:
  * [Windows](https://www.mongodb.com/docs/v4.4/tutorial/install-mongodb-on-windows-unattended/#run-mongodb-community-edition-as-a-windows-service):
    * In an Admin Command Prompt:
      * `net start MongoDB`, or
      * `net stop MongoDB`
    * Or, Open Task Manager > Services > MongoDB > Right Click > Start
  * [Linux](https://www.mongodb.com/docs/v4.4/administration/install-on-linux/)

* Deploy the project, for example on render.com, and get `LIVE_URL`.

* Set up `Sign in with Google`:
  * Create a Google Cloud Account and then a Google Cloud project.
  * Go to: Menu > API & Services > Credentials.
  * Click: Create Credentials > OAuth Client ID.
  * Follow on screen instructions:
    * Select Web Application for Application Type.
    * Add allowed origin: `LIVE_URL`
    * Add redirect URL: `LIVE_URL`/auth/google/articles
  * You will get `GOOGLE_CLIENT_ID` and `GOOGLE_CLIENT_SECRET`.

* Create a `.env` file in this directory, similar to the contents of `.env.example` file.
  - Set their values as you got using above steps.

* `npm install`

* `npm start`

## Technologies Used

EJS, Node.js, Express.js, MongoDB, Mongoose.js, Passport.js, Bootstrap, HTML, CSS, JS
