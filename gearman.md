### https://github.com/veny/GearmaNode
### https://github.com/mreinstein/node-gearman
### docker 
   ### url: https://hub.docker.com/r/mikolatero/gearman-job-server/
   ### setup gearman job server:   docker pull mikolatero/gearman-job-server
   ### Gearman job server over ubuntu 14.04
   #### Usage:
   #### If you want to deploy gearman with external access:
   #### docker run -d -p 4730:4730 --restart=always mikolatero/gearman-job-server 
   #### Or deploy gearman only with docker access:
   ##### docker run -d --restart=always mikolatero/gearman-job-server 
   #### You can change the external port change "-p 4730:4730" for any you want, for example: "-p 9999:4730" 
### github: 
#### https://github.com/mikolatero/docker-gearman-job-server
