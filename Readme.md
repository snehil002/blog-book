# BlogBook by Snehil: A Full Stack Online Blogging Platform

## Exciting Features
* Authentication
  * Login using Username and Password
  * Google Authentication
* CRUD - Create, View, Edit and Delete Articles

## How to Run this app?

* Install and Start MongoDB server locally (or online):
  * [Windows](https://www.mongodb.com/docs/v4.4/tutorial/install-mongodb-on-windows-unattended/#run-mongodb-community-edition-as-a-windows-service):
    * In an Admin Command Prompt:
      * `net start MongoDB`, or
      * `net stop MongoDB`
    * Or, Open Task Manager > Services > MongoDB > Right Click > Start
  * [Linux](https://www.mongodb.com/docs/v4.4/administration/install-on-linux/)

* Set up Google Sign In:
  * Create a Google Cloud Account and then a Google Cloud project.
  * Go to: Menu > API & Services > Credentials. Click: Create Credentials > OAuth Client ID.
  * Follow on screen instructions:
    * Select Web Application for Application Type.
    * Add Allowed Origin (domain) and redirect URL.
  * You will get GOOGLE_CLIENT_ID and GOOGLE_CLIENT_SECRET.

* Set the following environment variables:
  * Windows:
    * `SET SNEHIL_BLOG_PORT=<desired port number>`
      * Example: `SET SNEHIL_BLOG_PORT=4000`
    * `SET SNEHIL_BLOG_LIVE_URL=<live url of project with above port number (no trailing slash)>`
      * Example: `SET SNEHIL_BLOG_LIVE_URL=http://localhost:4000`
    * `SET SNEHIL_BLOG_MONGODB_URL=<url at which mongodb is running (no trailing slash)>`
      * Example: `SET SNEHIL_BLOG_MONGODB_URL=mongodb://127.0.0.1:27017`
    * `SET GOOGLE_CLIENT_SECRET=`
    * `SET GOOGLE_CLIENT_ID=`

  * Linux:
    * `export SNEHIL_BLOG_PORT=<desired port number>`
      * Example: `export SNEHIL_BLOG_PORT=4000`
    * `export SNEHIL_BLOG_LIVE_URL=<live url of project with above port number (no trailing slash)>`
      * Example: `export SNEHIL_BLOG_LIVE_URL=http://localhost:4000`
    * `export SNEHIL_BLOG_MONGODB_URL=<url at which mongodb is running (no trailing slash)>`
      * Example: `export SNEHIL_BLOG_MONGODB_URL=mongodb://127.0.0.1:27017`
    * `export GOOGLE_CLIENT_SECRET=`
    * `export GOOGLE_CLIENT_ID=`

* `npm install`

* `npm start`

## Technologies Used
EJS, Node.js, Express.js, MongoDB, Mongoose.js, Passport.js, Bootstrap, HTML, CSS, JS
