# innerloop

#
# SETUP
#

Assuming that the following are already installed:
- jdk
- oc
- odo
- VS Code

Start.spring.io
	- Create a basic rest service
	- spring web as a dependency
Decompress

Create project in github (empty, Java)
Git clone project to local machine

Move contents of spring project to the git clone folder
Add contents to project and commit as initial revision

Log into openshift
Create project called innerloop
Login from command line and change to innerloop project
Oc project innerloop


# 
# ADD SERVICE
# 

 odo create java-springboot innerloop 
 odo push

open url and see a not found error
curl http://8080-tcp-app-innerloop.apps.ocp4.home.glroland.com/
{"timestamp":"2022-02-13T16:42:56.446+00:00","status":404,"error":"Not Found","path":"/"}%               

 add a rest operation that says hello
 --sample operation is in this project under Hello controller

 odo push

 open url again
 http://8080-tcp-app-innerloop.apps.ocp4.home.glroland.com/
result should say hello

