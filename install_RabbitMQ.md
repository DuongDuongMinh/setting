# install rabbit mq
# reference 
### https://www.tutlane.com/tutorial/rabbitmq/rabbitmq-installation

### https://dev.to/jay97/docker-compose-an-express-and-mongo-app-aai

### https://medium.com/swlh/a-practical-guide-for-jwt-authentication-using-nodejs-and-express-d48369e7e6d4

### https://dev.to/medaymentn/securing-your-node-js-api-with-json-web-token-5o5

### https://nordicapis.com/why-cant-i-just-send-jwts-without-oauth/?source=post_page

### http://travistidwell.com/jsencrypt/demo/?source=post_page

### http://expressjs.com/en/resources/middleware/multer.html

# header
#### 1.docker-compose, docker-manager
#### 2.jsonwebtoken
# 3.express
# 4.router
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
