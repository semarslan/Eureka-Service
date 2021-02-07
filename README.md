# Eureka-Service

### Run eureka-service first, then the others in order

2. https://github.com/semarslan/Cloud-Config-Server

3. https://github.com/semarslan/Cloud-Gateway-Service

4. https://github.com/semarslan/Department-Service

5. https://github.com/semarslan/User-Service

### Department Service:

Create Department -- 

http://localhost:9191/departments 

{
	"departmentName" : "IT",
	"departmentAddress" : "test address",
	"departmentCode" : "IT-006"
}

Get Department By Id : http://localhost:9191/departments/1

### User service: 

Create User --

http://localhost:9191/users

{
	"name" : "sema",
	"lastName" :"ars",
	"email" : "test@test.c",
	"departmentId" : "1"
}

Get User By Id: http://localhost:9191/users/1

------------

## https://github.com/semarslan/config-server this repo is used. Because eureka-server integration is here.
