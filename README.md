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
![image](https://github.com/shlhs/monitor_screen_release/blob/master/pic/monitor_screen_table.jpg)

#### redis

### 启动命令，参数根据实际情况修改或添加：
nohup java -jar monitor-screen-0.2.jar --spring.datasource.url=jdbc:mysql://114.25.9.8:4408/lhs_cloud_collector?useUnicode=true\&characterEncoding=utf-8 --spring.datasource.username=dadadad --spring.datasource.password=dadad --spring.redis.host=114.12.21.21 --spring.redis.port=6379 --spring.redis.password=21312 --server.port=9191 &

        
[运行包 下载地址](https://github.com/shlhs/monitor_screen_release/blob/master/dist/monitor-screen-0.2.jar)  

### 测试链接：
http://ip:port/monitor_screen?sn=AVQPEAQH

    
注：这里的画面sn（AVQPEAQH）, 根据实际情况进行替换；不同画面, sn不同，该关系存储在MySQL中。


### 默认参数：
```java
server.port=8098

# REDIS (RedisProperties)
spring.redis.database=0
spring.redis.host=47.93.32.6
spring.redis.port=6379
spring.redis.password=
spring.redis.pool.max-active=-1
spring.redis.pool.max-wait=-1
spring.redis.pool.max-idle=8
spring.redis.pool.min-idle=0
spring.redis.timeout=0
spring.thymeleaf.mode=LEGACYHTML5

#spring.datasource.url=jdbc:mysql://127.0.0.1:3306/simufiled
spring.datasource.url=jdbc:mysql://172.17.233.75:4408/collector?useUnicode=true&characterEncoding=utf-8
spring.datasource.username=2312313
spring.datasource.password=21323
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
