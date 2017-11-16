# api-workshop-107_zipkin_server

Build ZipKin-Server

1. add dependencies


	compile('org.springframework.boot:spring-boot-starter-actuator')
	compile('org.springframework.boot:spring-boot-starter-aop')
	compile('org.springframework.cloud:spring-cloud-sleuth-stream')
	compile('org.springframework.cloud:spring-cloud-sleuth-zipkin-stream')
	compile('org.springframework.cloud:spring-cloud-starter-sleuth')
	compile('org.springframework.cloud:spring-cloud-stream-binder-rabbit')
	compile('org.springframework.boot:spring-boot-starter-web')
	runtime('io.zipkin.java:zipkin-autoconfigure-ui')

2. config properties


    server.port=20000
    spring.application.name=zipkin-server
    
3. add annotation 


    @EnableZipkinServer
    
4. access 

    
    http:localhost:2000