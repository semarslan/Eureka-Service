# Eureka-Service

### Run eureka-service first, then the others in order


2. https://github.com/semarslan/Cloud-Config-Server 

3. https://github.com/semarslan/Cloud-Gateway-Service

4. https://github.com/semarslan/Department-Service

5. https://github.com/semarslan/User-Service

6. https://github.com/semarslan/Hystrix-Dashboard


-----------

## Zipkin Server:

docker run -d -p 9411:9411 openzipkin/zipkin

url: http://localhost:9411/zipkin


-------------------

* eureka server: localhost:8761
* hystrix-dashboard: localhost:9295/hystrix
* api-gateway: localhost:9191/actuator/hystrix.stream


* Department Service:

Create Department -- 

http://localhost:9191/departments 

{
	"departmentName" : "IT",
	"departmentAddress" : "Ankara",
	"departmentCode" : "IT-06"
}

Get Department By Id : http://localhost:9191/departments/1

* User service: 

Create User --

http://localhost:9191/users

{
	"name" : "sema",
	"lastName" :"arslan",
	"email" : "94.sema.arslan@gmail.com",
	"departmentId" : "1"
}

Get User By Id: http://localhost:9191/users/1

------------

## https://github.com/semarslan/config-server this repo is used. Because eureka-server integration is here.



