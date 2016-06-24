################################################################
##
## PURPOSE:
## customized tomcat server for maven deployments
##
## HISTORY:
## 5:03 PM 4/20/2015 created 
##
## PREREQUSITES:
## 1. <none>
##
################################################################
FROM tomcat:8-jre8
MAINTAINER "Zeljko Gavrilovic <zeljko.m.gavrilovic@gmail.com>"
RUN mkdir -p /usr/local/tomcat/conf
ADD settings.xml 		/usr/local/tomcat/conf/
ADD tomcat-users.xml 	/usr/local/tomcat/conf/
COPY target/dockerapp.war /usr/local/tomcat/webapps/
