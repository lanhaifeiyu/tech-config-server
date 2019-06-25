# tech-config-server
tech-config-server

config-server:
http://localhost:9002/tech-blog-provider/dev/master
config-server项目需要注入eureka-client，不然不能自动刷新

config client项目（tech-blog）：
执行POST请求刷新配置：http://localhost:8888/actuator/refresh
访问配置数据：http://localhost:8888/getConfigInfo
执行POST请求刷新配置(amqp bus fresh): http://localhost:9002/actuator/bus-refresh

