
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


