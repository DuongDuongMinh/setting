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
### 14. https://medium.com/@technospace/an-introduction-to-oauth-2-0-4c71b5fb19ff


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
#### 6.https-error
# 7.cors
#### 8.eslint
# 9.mocha test
# 10. .editorconfig
# 11. .evn
# 12.redis
#### 13.prettierrc
#### 14.promise
# 15.sails
# 16.auth2.0
#### 17.callback
#### 18. .gitignore
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
#### 37. morgan
# 38. axios.
# 39. fb.
# 40. google-auth-library
# 41. blubird.
# 42. pg
# 43. jset
#### 44. prettier.
# 45. supertest
# 46. precommit


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
```
## RESTful API.
## MYSQL
## firebase.
## socket
## unitest nhat gui.
## sensui / the-craftsman-book
## rabbitmq
## radis
## mongodb, kapka
## kapka with uber
## https://medium.com/@WSO2/guidelines-for-designing-microservices-71ee1997776c
## microservice
## cloud store blackblaze
## (ElasticSearch, Cassandra)
##  Kong API Gateway
## bitbucket.
## confluence
## zeplin
## jira software
## kong
## nginx
## docker

### important system architecture.
### what webserver.
## job server.
### caching
## services
### cloud store.
### loadbalance.
### fulltext search service
### data machine.
### cdn
### dns
### https://codeburst.io/what-is-a-web-server-97362996d229
### https://engineering.videoblocks.com/web-architecture-101-a3224e126947
### https://medium.com/@utkarsh_verma/configure-nginx-as-a-web-server-and-reverse-proxy-for-nodejs-application-on-aws-ubuntu-16-04-server-872922e21d38

### https://blog.sourcerer.io/apache-is-still-the-best-general-purpose-web-server-dacedbd86921
# web server.. nginx, redis mongo db
### https://medium.com/quick-code/top-tutorials-to-learn-nginx-for-web-server-dc8638c48fae
### https://medium.com/@fermads/node-js-process-load-balancing-comparing-cluster-iptables-and-nginx-6746aaf38272
### https://medium.com/better-programming/implementing-rabbitmq-with-node-js-93e15a44a9cc
### https://medium.com/@freekmurze/load-balancing-with-nginx-95d902b4849f

### https://medium.com/@auth0/load-balancing-node-js-applications-with-nginx-and-docker-1739e0cec2ef
### https://medium.com/signal-sciences-labs/securing-microservices-and-apis-with-nginx-and-signal-sciences-17904d3a830a
### https://medium.com/better-programming/implementing-rabbitmq-with-node-js-93e15a44a9cc

### https://itnext.io/request-id-tracing-in-node-js-applications-c517c7dab62d

### https://medium.com/hackernoon/scaling-node-js-socket-server-with-nginx-and-redis-d19bf5c07fa8

# firebase
### https://blog.usejournal.com/build-a-serverless-full-stack-app-using-firebase-cloud-functions-81afe34a64fc
### https://medium.com/hackernoon/nodejs-setup-firebase-in-4-step-tutorial-example-easy-beginner-service-account-key-json-node-server-d61e803d6cc8
### https://codeburst.io/how-to-build-a-command-line-app-in-node-js-using-typescript-google-cloud-functions-and-firebase-4c13b1699a27

### https://auth0.com/blog/how-to-authenticate-firebase-and-angular-with-auth0-part-1/?utm_source=medium&utm_medium=sc&utm_campaign=firebase_angular

### https://medium.com/@JamWils/keeping-the-realtime-in-firebases-realtime-database-ed60bddbee90


# database
### heap meaning.
### vertical scale.
### horizontal scale.
### https://en.wikipedia.org/wiki/Multiversion_concurrency_control

# type database and storage engine
### http://www.mysqltutorial.org/wp-content/uploads/2018/03/MySQL-Storage-Engines-Feature-Summary.pdf
### http://www.mysqltutorial.org/wp-content/uploads/2018/03/MySQL-Data-Types.pdf




Phần quan trọng nhất là phải đọc documentation. sau đó là suy nghĩ cách giải quyết. 10% là code. nhưng lại chiếm 90% thời gian.(lãng phí đó).
### hãy nhớ là giống với lau nhà vậy 90% thời gian là chuẩn bị và lau dọn bàn ghế bụi bẩn. duy chỉ có 10% là thời gian dùng để lau sàn nhà.
### nếu trong lập trình mình dành 10% thời gian đó làm đầu tiên. Vậy như là đi lau nhà trước trong khi việc khác làm sau thì cả căn nhà vẫn bẩn bình thường vì lau. lau  mọi thứ xuống. sàn nhà sẽ bị dơ. ta đã lãng phí 10% thời gian lau sàn. Thêm việc lại mất 10% thời gian lau lại. Mà nhiều lúc ta lại quan tâm xem sàn của ta có dơ không. vậy phải mất thêm 30_ 50% thời gian cho việc đó. --> tới việc làm lau những thứ khác k sạch sẽ. vậy thời gian ta lãng phí quá nhiều rồi...vậy mất 90% thời gian chỉ để làm 1 việc trong khi chỉ cần 10% là hoàn thành nếu ta biết chuẩn bị tài liệu trước, đưa ra phương hướng, nghĩ ra tất cả khả năng xảy ra, hình thành tư duy sắp xếp hệ thống, thứ tự trước sau. Thì 10% lần sau ta làm rất đơn giản.
Những bước chuẩn bị và xác định phương hướng sẽ chiếm 90% thời gian đủ để ta suy nghĩ và đưa ra phương án tốt nhất. Đó là con đường mà mình nên đi. Học code là để suy nghĩ và cách tổ chức hệ thống khi mình chưa biết. Còn nếu trong dự án. thì phải có con mắt nhà kinh tế. phài tư duy quan sát. 10% thời gian còn lại cuối cùng là trình bày ra sản phẩm mà mình đã có kế hoạch đã có sự chuẩn bị trước đó. ok
