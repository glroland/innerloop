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
	- Jersey as a dependency
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
# ADD AND USE
# 

 odo create java-springboot innerloop 
 odo push

 open url and it should show the old tomcat style not found page
 http://8080-tcp-app-innerloop.apps.ocp4.home.glroland.com/

 add a rest operation that says hello
 --sample operation is in this project under Hello Resource

 odo push

 open url again
 http://8080-tcp-app-innerloop.apps.ocp4.home.glroland.com/

