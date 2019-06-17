# Java使用Redis实现发布与订阅


### 1.安装redis
````
docker pull redis
docker run -d --name redis  -p 6379:6379 redis
````

### 2.编译
````
cd java-redis-pub-sub
mvn install
````

### 3.启动订阅程序
````
mvn exec:java -Dexec.mainClass="com.frontng.demo.redispubsub.Sub"
````

### 4.启动发布程序
````
mvn exec:java -Dexec.mainClass="com.frontng.demo.redispubsub.Pub"
````