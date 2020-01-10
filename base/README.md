
#　dst-docker启动流程
需要安装```docker 以及 docker compose```环境

１、　将打包好的```dst.jar```放入当前目录

２、　修改```docker-compose.yaml```中的变量.

* ```mem_limit```设置docker容器大小，```JAVA_OPTS```设置java的启动参数

* 默认的docker容器大小1G,java启动内存820Ｍ

３、　在当前目录执行shell：启动：```docker-compose up -d```
* 查询　```docker-compose　ps``` 
* 停止　```docker-compose stop```
* 状态监控：　```docker stats```
* 进入docker容器：```docker exec -it dst bash```
