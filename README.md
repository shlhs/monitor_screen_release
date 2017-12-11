# monitor_screen_release
## How to deploy?
### 运行环境：
jre 1.8   
java -version    
java version "1.8.0_20"    
Java(TM) SE Runtime Environment (build 1.8.0_20-b26)    
Java HotSpot(TM) 64-Bit Server VM (build 25.20-b23, mixed mode)

### 依赖周边组件：
#### mysql


#### redis

### 启动命令，参数根据实际情况修改或添加：
java -jar /home/pvweb/pv-web-0.1.0.jar  --server.port=8090 --spring.datasource.url=jdbc:mysql://127.0.0.1:3306/dty --spring.datasource.username=root --spring.datasource.password=xxxxxx

### 测试链接：
http://ip:port/monitor_screen?sn=AVQPEAQH
注：这里的画面sn（AVQPEAQH）, 根据实际情况进行替换；不同画面, sn不同，该关系存储在MySQL中。


### 默认参数：
```java
server.port=8080

# REDIS (RedisProperties)
spring.redis.database=0
spring.redis.host=114.215.9.8
spring.redis.port=6379
spring.redis.password=
spring.redis.pool.max-active=-1
spring.redis.pool.max-wait=-1
spring.redis.pool.max-idle=8
spring.redis.pool.min-idle=0
spring.redis.timeout=0
spring.thymeleaf.mode=LEGACYHTML5

#spring.datasource.url=jdbc:mysql://127.0.0.1:3306/simufiled
spring.datasource.url=jdbc:mysql://114.215.90.83:3306/dty
spring.datasource.username=root
spring.datasource.password=xxxxxx
spring.datasource.driver-class-name=com.mysql.jdbc.Driver
spring.datasource.driver-class-name=com.mysql.jdbc.Driver
spring.datasource.max-idle=10
spring.datasource.max-wait=10000
spring.datasource.min-idle=5
spring.datasource.initial-size=5
spring.datasource.validationQuery=select 1
spring.datasource.testWhileIdle=true
spring.datasource.timeBetweenEvictionRunsMillis=300000
spring.datasource.minEvictableIdleTimeMillis=600000

```
