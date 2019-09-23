
https://www.robinwieruch.de/prettier-eslint/
https://prettier.io/docs/en/integrating-with-linters.html

## UML
https://diagrams.visual-paradigm.com/#diagram:proj=0&type=SequenceDiagram&gallery=/repository/cd35ced7-7ffc-47c2-bfb5-69a5b6d3b1bb.xml&name=Loop%20Fragment
## git undo
https://kipalog.com/posts/Undo--mot-commit-trong-git-tree
https://kbroman.org/github_tutorial/pages/first_time.html

## jwt auto key
http://travistidwell.com/jsencrypt/demo/?source=post_page
https://github.com/auth0/node-jsonwebtoken/issues/336

## facebook
https://developers.facebook.com/apps/684348638658023/fb-login/settings/

## socket
https://medium.com/containers-on-aws/scaling-a-realtime-chat-app-on-aws-using-socket-io-redis-and-aws-fargate-4ed63fb1b681

## redis
## sudo service redis-server restart
https://redislabs.com/blog/redis-on-windows-10/

https://blog.ndk.name/change-mysql-server-authentication-plugin-for-root-user/

https://o7planning.org/vi/11959/ket-noi-co-so-du-lieu-mysql-su-dung-nodejs

https://github.com/nodejs/help/issues/134


## sql with timeout
https://sequelize.org/master/manual/hooks.html#declaring-hooks
xampp.org
https://bitbucket.org/comspacesphotosystem/comspace-community/src/master/

http://www.mysqltutorial.org/mysql-order-by/

mysqladmin -u root password [newpassword]
mysql -u root -p
https://github.com/mysqljs/mysql#connection-options

## Giả sử khi ta tạo nên 1 verify_code đi phải cho nó khoảng thời gian kết thúc. ví dụ như sau.
code  = 12345;
code -> save to database ...sau đó sẽ có 1 function là settimeout...(cài khoảng thời gian đặt lại code='') có nghĩa là code đó sẽ mất hiệu lực trong khoảng thời gian là bao lâu. ok.

## when you use dev or product environment.

### resful and asnyc and one thread

https://backendapi.turing.com/docs/
https://www.sohamkamani.com/about

https://towardsdatascience.com/getting-started-with-git-and-github-6fcd0f2d4ac6

https://medium.com/better-programming/is-javascript-synchronous-or-asynchronous-what-the-hell-is-a-promise-7aa9dd8f3bfb

### unitest
https://github.com/sensui/the-craftsman-book?fbclid=IwAR2u3xDUOZbkO8o6jbtqISr-oICRM5udtzMNk2RTGqilartI5mrw8byfLGE


### rabbitms

I had the same Problem..

I installed RabbitMQ and Enabled Web Interface also but still couldn't sign in with any user i newly created, this is because you need to be administrator to access this.

Do not create any config file and mess with it..

This is what i did then,

Add a new/fresh user, say user test and password test:

rabbitmqctl add_user test test
Give administrative access to the new user:

rabbitmqctl set_user_tags test administrator
Set permission to newly created user:

rabbitmqctl set_permissions -p / test ".*" ".*" ".*"
That's it, enjoy :)
https://www.squaremobius.net/amqp.node/channel_api.html

### uber
https://eng.uber.com/ureplicator/
https://www.slideshare.net/zhenxiao/machine-learning-and-big-data-uber-a-tale-of-two-systems
### hoat dong dieu khien tu xa.
kafka, mongodb(???), rabbitmq, mysql

 mỗi 1 server sẽ nói chuyện với nhau theo 2 cách. Cách 1 là qua sync và cách hai là qua async, cách 3 là tự nói chuyện 1 mình cho mình tự hiểu.
 ví dụ như chiếc máy tính, nói chuyện theo sync là qua dây nối hai thằng máy tính với nhau(hai thằng ở gần).
vậy 2 thằng ở xa thì phải nói chuyện qua internet và có 1 kênh trung gian để hai thằng nói chuyện giống zalo vậy.
cách 3 là tự mình xử lý hay sử dụng ứng dụng trên máy tính của mình..tự chơi 1 mình.


ví dụ mình có thể nói chuyện với đứa hàng xóm vì nó gần nhà....vậy thì (asyn) điều kiện là nhà gần nhau, nói trực tiếp.
mình nói chuyện với một thằng ở mỹ thì mình phải nói qua phương tiện trung gian khác, ví dụ thư điện tử, zalo hay cái gì đó.
hoặc mình tự nói mình nghe...


- rabbit mq thì tất cả con rabbitmq đều có thể nói chuyện với nhau thông qua 1 cổng chung chẳng hạn amqp:hieu@localhost...
ví dụ hiếu cũng dùng rabbit mq. và kết nối qua cổng này, hội cũng vậy và mình cũng vậy thì bây giờ 3 đứa nói chuyện với nhau ở đây.
- tiếp giờ hội dùng webser, hiếu dùng 1 cái database, mình dùng 1 webserver đi.. vậy cả 3 người muốn nói chuyện với nhau thì qua rabbitmq.
nhưng mình và hội lại cùng dùng webserver...cùng kết nối là http://comspaces/* gì đó.
vậy mình và hội có thể nói chuyện tại đây, hội là keenhh /nghia mình có kênh là /minhchau...
hội có thể gọi tên mình /minhchau, minhc có thể gọi tên hôi là /nghia. 


* chú ý nếu như cả mình, nghĩa và hiếu cùng dùng rabbitmq để tạo exchange, queue chẳng hạn thì cái rabbitmq này k khác gì 1 cái webserver nếu ta lên hẳn cái trang web hiểu thị tạo thư exchane, hoặc queue...
nhưng là 1 api server khi ta sử dụng dòng lệnh. lúc đó k có giao diện gì cả... 
rabbitmq thì cũng giống với mình dùng 1 trang web..
mình tới địa chỉ trang web nào.. url...
tiếp theo là 1 là khách hai là thành viên. (thành viên thì có password và username) mỗi cái tài khoản sẽ có thông tin bảo mật của mình ha.. vậy thì mình dùng nó rồi... thông tin mình cho nên đó. mình muốn cho ai vào thì cho người ta mật khẩu, hoăc có thể vào 1 nhóm chát với nhau đó.. trong đó có chứa dữ liệu mà cả 3 người cùng thao tác được.

### mongodb
https://www.objectrocket.com/blog/mongodb/intro-to-massive-scaling-with-mongodb/


### log
https://engineering.linkedin.com/distributed-systems/log-what-every-software-engineer-should-know-about-real-time-datas-unifying?fbclid=IwAR0ks_9xwyrc7KgOS8GpaUIcqVtkgWIxIu9oNDywQmo1OI4qF2mMTf1F_Io

### kafka
https://engineering.linkedin.com/blog/2016/04/kafka-ecosystem-at-linkedin
### AI
https://conferences.oreilly.com/artificial-intelligence/ai-ny-2018/public/schedule/detail/65105

### docker and hadoop, microservice, loadbalance, realtime
### system design
https://medium.com/@narengowda/uber-system-design-8b2bc95e2cfe
### facebook
https://medium.com/@shagun/scaling-memcache-at-facebook-1ba77d71c082

### nginx

https://www.tecmint.com/nginx-web-server-security-hardening-and-performance-tips/
https://www.tecmint.com/nginx-web-server-security-hardening-and-performance-tips/

https://dev.to/guimg/how-to-serve-nodejs-applications-with-nginx-on-a-raspberry-jld
https://www.tecmint.com/nginx-web-server-security-hardening-and-performance-tips/

### nginx 
https://blog.cloudflare.com/

https://themeisle.com/blog/prevent-image-hotlinking-in-wordpress/

https://en.wikipedia.org/wiki/MD5

https://en.wikipedia.org/wiki/Cryptographic_hash_function
https://en.wikipedia.org/wiki/RPM_Package_Manager
https://en.wikipedia.org/wiki/Yum_(software)
https://unit.nginx.org/installation/

https://www.siteground.com/themeisle?afcode=b1d0f6820e046c19802d21f3b46eb61d&campaign=ti-filezilla

https://techmaster.vn/posts/34635/gioi-thieu-ve-nginx-cho-lap-trinh-vien?fbclid=IwAR3UVQodidUtnr5JXIrv_-aSBew9ugymXQsrMbJFMrOJVxG7H-De4Y2vhyA

https://serverguy.com/comparison/apache-vs-nginx/?fbclid=IwAR2Iht6lAEphhpk6KGOCtpnMpf5VeHipAu8BknbgQtIY4r59BO96ovUudhQ

https://www.freecodecamp.org/news/

### directory ubuntu
https://askubuntu.com/questions/759880/where-is-the-ubuntu-file-system-root-directory-in-windows-subsystem-for-linux-an

https://demo.nginx.com/swagger-ui/?_ga=2.227511386.614264120.1567763976-2023068060.1567594320#/General_Info/getNginx
### .env
https://medium.com/the-node-js-collection/making-your-node-js-work-everywhere-with-environment-variables-2da8cdf6e786

### date-time
``` node.js
I don't think toJSON is implemented in IE, so I don't think we should use that. It looks like the native Date object uses ISO8607, so maybe we could just use that.

(new Date()).toJSON(); // "2012-09-24T17:16:42.483Z"
I'll look into the details of Date.prototype.toJSON, but I think one of the following should work.

// just use the default ISO8607 that moment uses
moment.fn.toJSON = function () {
    return moment.utc(this).format();
}
// use the ISO8607 that Chrome uses
moment.fn.toJSON = function () {
    return moment.utc(this).format('YYYY-MM-DD[T]HH:mm:ss.SSS[Z]');
}
```
https://momentjs.com/docs/

### request
https://github.com/request/request
https://www.npmjs.com/package/request

### blog it
https://itviec.com/blog/9-tech-blogger-the-gioi-ban-can-biet/

### kong
https://konghq.com/faqs/
https://medium.com/@far3ns/kong-the-microservice-api-gateway-526c4ca0cfa6
https://puppet.com/docs/pipelines-for-apps/enterprise/application-nodejs-mocha.html


### search and another tutorial best
https://codeforgeek.com/mongodb-elasticsearch-synchronization/

### deploy
https://puppet.com/docs/pipelines-for-apps/enterprise/manifest.html

### await
https://blog.bitsrc.io/understanding-javascript-async-and-await-with-examples-a010b03926ea

### restful
patch https://medium.com/backticks-tildes/restful-api-design-put-vs-patch-4a061aa3ed0b

### search full text
https://www.tunglt.com/2018/11/bo-dau-tieng-viet-javascript-es6/
https://medium.com/@nickgerleman/the-bkd-tree-da19cf9493fb
https://en.wikipedia.org/wiki/K-D-B-tree
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/normalize
very good: elastic.co

### firebase
var firebaseConfig = {
  apiKey: "api-key",
  authDomain: "project-id.firebaseapp.com",
  databaseURL: "https://project-id.firebaseio.com",
  projectId: "project-id",
  storageBucket: "project-id.appspot.com",
  messagingSenderId: "sender-id",
  appID: "app-id",
};
is public all the world so you need security for this to filebase project.
if not security all peopler can add their app to your filebase project.

security:::::
https://firebase.google.com/docs/firestore/security/get-started
https://firebase.google.com/docs/database/security/quickstart
https://firebase.google.com/docs/database/security/quickstart
https://firebase.google.com/docs/storage/security/start

MQTT

- you need to setup secure for database because all people can read and write your data, even people not use your app.

https://www.google.com/search?sxsrf=ACYBGNQq_eXbcPvVLB-IIx657DzDmyINWA%3A1568857499721&ei=m92CXf3EK9mpoATEhpqYCg&q=set+up+firebase+rules&oq=set+up+firebase+rules&gs_l=psy-ab.3...2201.7836..8344...2.1..0.140.1996.16j6......0....1..gws-wiz.....10..0i71j35i362i39j35i39j0j0i131j0i67j0i203j0i10i203j0i22i30j33i22i29i30.Xi-WrUccwkw&ved=0ahUKEwi9_uTP4dvkAhXZFIgKHUSDBqMQ4dUDCAs&uact=5#kpvalbx=_pd2CXdOSM9CmoATYlI2ACA23

### server
giả sử có 10 conserver thì lúc nào cũng bật rồi.
1 cón sẽ có cổng 127.09.08
con thư 2 có công 127.09.09
....
mỗi con thì như la 1 chiếc máy tính. mỗi máy tính thì có thể chay nhiều ứng dụng web
chỉ cần khác port là được
giả sử 1 con server có phục vụ 10000 người chẳng hạn, thì sẽ có port là 2000, 2001, 20002 ....vân vân.
khi mà 1 người có 1 lời gọi thì 
- bước 1 nginx sẽ phân cho 1 server(máy chủ host) rồi mỗi máy chủ sẽ tự động bật lên 1 port. khi khác hàng logout hoặc ngắt kết nối thì port nó sẽ tắt kết nối.
mỗi khách hàng khác lại vào thì nó lại bật lên.....
nếu server này mà đầy rồi, thì ngixn phân sang server khách chưa đầy. Nếu tất cả full thì phải ngồi đợi thôi.
giống phòng game vậy đó.
server là 1 phòng. mỗi máy tính là port. 1 người chơi vào thì bật máy. k chơi nữa thì tắt máy. người mà đang sắng màn, thì vẫn chơi. ok.

### axios:
rest in firebase

https://howtofirebase.com/collection-queries-with-firebase-b95a0193745d
https://softauthor.com/firebase-querying-sorting-filtering-database-with-nodejs-client/
https://arduino.esp8266.vn/network/mqtt.html
https://code.google.com/archive/p/mqtt4erl/wikis/QualityOfServiceUseCases.wiki

### socket..
https://cdnjs.com/libraries/socket.io
server side
 #### 1. http
 #### 2. cmqp
 ##### 3. tcp
 #### 4. long polling
 #### 5. short polling
 #### 6. websocket.
 #### google analyn
 ### user_angel_chome
 ### console for check sesource
 
### amqp
### protocal ????
### http
#### tcp
#### resever server
###  server side
### 
https://www.jeffalytics.com/ip-tracking-google-analytics/
