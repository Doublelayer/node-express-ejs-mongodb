# Node-Express-MongoDB - Boilerplate

### The following Instructions are to start from scratch without cloning this boilerplate.
### If you don't need it then just clone this repo and have fun

# 1. cloning

- [ ] git clone 
- [ ] cd node-express-mongodb 
- [ ] npm init -y 

# 2. dependencies

- [ ] npm i express ejs express-ejs-layouts
- [ ] npm i --save nodemon // restart npm server automaticlly
- [ ] configure package.json

- "scripts":{
  "start": "node server.js",
  "dev": "nodemon server.js"
  }
- "main": "server.js"

# 3. server.js

- [ ] use express
- [ ] set view enginge : "ejs"
- [ ] set views : \_\_dirname + "/views"
- [ ] use layout : layouts/layout
- [ ] use express.static("public")
- [ ] listen => process.env.PORT // production|| 3000

# 4. first test

- [ ] npm run dev // localhost:3000

# 5. routes (controller)

- [ ] create routes folder
- [ ] create index.js file
- [ ] import express
- [ ] create router from express
- [ ] router.get on "/" => res.send("")
- [ ] export router
- [ ] in server.js import routes/index

==> now you should see your send object!

# 6. layout

- [ ] create layouts folder inside views
- [ ] create layout.ejs file inside layouts
- [ ] type ! and than press enter to generate template html
- [ ] inside body implement <%- body %>
- [ ] create index.ejs file inside views
- [ ] write your text you want to import inside index.ejs (e.g. Hello World)

==> now yout should see you text on root

# 7. mongoDB

- [ ] npm i --save-dev dotenv
- [ ] create .env file (DATABASE_URL = mongodb://localhost/db)
- [ ] npm i mongoose (used version: 5.6.0)
- [ ] import mongoose inside server.js
- [ ] import dotenv.config
- [ ] connect mongoose to process.env.DATABASE_URL
- [ ] get db object form mongoose.connection
- [ ] create on error handler
- [ ] create once on open

# 8. deployment

- [ ] go to "https://www.heroku.com/"
- [ ] create a account
- [ ] create new app
- [ ] in section "deployment method" click on GitHub and connect yout repo with heroku
- [ ] choose between "Enable auto deploys" || "Manual deploy"
- [ ] finally click on "deploy branch"
- [ ] finally click on "View" ==> you will see an error!
- [ ] create accoutn on "https://cloud.mongodb.com/" => create clutster => create collection
- [ ] create a user
- [ ] get the connection string and paste user credentials
- [ ] add enviroment variable ==> settings => reveal config vars
- [ ] DATABASE_URL : <connection-string>
