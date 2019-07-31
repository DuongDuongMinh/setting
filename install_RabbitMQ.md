# install rabbit mq
# reference 
### https://www.tutlane.com/tutorial/rabbitmq/rabbitmq-installation

### https://dev.to/jay97/docker-compose-an-express-and-mongo-app-aai

### https://medium.com/swlh/a-practical-guide-for-jwt-authentication-using-nodejs-and-express-d48369e7e6d4

### https://dev.to/medaymentn/securing-your-node-js-api-with-json-web-token-5o5

### https://nordicapis.com/why-cant-i-just-send-jwts-without-oauth/?source=post_page

### http://travistidwell.com/jsencrypt/demo/?source=post_page

### http://expressjs.com/en/resources/middleware/multer.html


# today: 
### 1. https://medium.com/hackernoon/async-testing-koa-with-jest-1b6e84521b71
### 2. https://medium.com/@grantminer/why-you-should-use-koa-with-node-js-7c231a8174fa
### 3. https://medium.com/javascriptjedi/middleware-in-nodejs-8623cb6cff7
### 4. https://medium.com/@Abazhenov/using-async-await-in-express-with-node-8-b8af872c0016
### 5. https://medium.com/@simov/oauth-like-a-boss-e336f6a7e149
### 6. https://medium.com/@tarkus/how-to-open-database-connections-in-a-node-js-express-app-e14b2de5d1f8
### 7. https://medium.com/@carlos.illobre/nodejs-express-how-to-organize-your-routes-in-very-big-applications-and-why-controllers-are-evil-e202eea497f4
### 8. https://medium.com/netscape/mastering-koa-middleware-f0af6d327a69
### 9. https://codeburst.io/build-a-weather-website-in-30-minutes-with-node-js-express-openweather-a317f904897b?gi=9cf11ec46af1
### 10. https://medium.com/@jonm90/express-to-koa-learn-koa-express-3132ad539b4f
### 11. https://medium.com/@purposenigeria/build-a-restful-api-with-node-js-and-express-js-d7e59c7a3dfb
### 12. https://medium.com/silibrain/using-passport-bcrypt-for-full-stack-app-user-authentication-fe30a013604e
### 13. https://medium.com/@therealchrisrutherford/nodejs-authentication-with-passport-and-jwt-in-express-3820e256054f


## eslint 
### 15. https://scotch.io/tutorials/code-formatting-with-prettier-in-visual-studio-code
### 16. https://scotch.io/tutorials/linting-and-formatting-with-eslint-in-vs-code

## architecture
### 17. https://dev.to/santypk4/bulletproof-node-js-project-architecture-4epf


### 29. https://medium.com/@raygunio/hapi-vs-express-in-2018-node-js-framework-performance-comparison-e68293b10a36
### 30. https://medium.com/@stockholmux/redis-express-and-streaming-with-node-js-and-classic-literature-d00f13368db3


# project 
## https://medium.mybridge.co/45-amazing-node-js-open-source-for-the-past-year-v-2019-c774d750e925


# header
#### 1.docker-compose, docker-manager
#### 2.jsonwebtoken
#### 3.express
#### 4.router
# 5.koa
# 6.https-error
# 7.cors
# 8.eslint
# 9.mocha test
# 10. .editorconfig
# 11. .evn
# 12.redis
# 13.prettierrc
# 14.promise
# 15.sails
# 16.auth2.0
# 17.callback
# 18. .gitignore
# . cache...
# 20.login with google
# 21 login with facebook
# 22. node-fetch for login
# 23. login with linkedin
# 24. login with twitter
#### 25.-rabbitmq 
#### 26. mongodb-
#### 27. swagger-
# 28. ramda
#### 29. nodejs restful api-
# 30. winston
# 31. ajv
# 32. config
# 33. crypto
# 34. bcryptjs
# 35. helmet
# 36. knex.
# 37. morgan
# 38. axios.
# 39. fb.
# 40. google-auth-library
# 41. blubird.
# 42. pg
# 43. jset
# 44. prettier.
# 45. supertest

Note: router, subapp(amout) or callback...
example... 
```node.js
var express = require('express');
var app = express();
var subapp = express();

//subapp.
subapp.get('/product1', (req, res) => {
   if(req.body.number > 2){
      console.log('subapp');
   }
}
app.use('/api', subapp);

app.listen(3000, () => {
  console.log('web server listens port 3000);
});

//===> subapp...will mount app...example /api/proudct1..
//we will use.. all of the things subapp do that will same router(= express.Router());

//router and subapp, have call back and functions same app./...the same app..
