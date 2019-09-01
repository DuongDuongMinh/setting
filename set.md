
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


## sql
https://sequelize.org/master/manual/hooks.html#declaring-hooks
xampp.org
https://bitbucket.org/comspacesphotosystem/comspace-community/src/master/

http://www.mysqltutorial.org/mysql-order-by/

mysqladmin -u root password [newpassword]

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
