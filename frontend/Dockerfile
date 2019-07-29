#This is Docker file
#FROM
#MAINTAINER
#RUN
#ADD
#COPY
#ENV
#EXPOSE
#CMD
#ENTRYPOINT
#USER
#WORKDIR
#ARG
#VOLUME
# pull centos:7
#Update of all existing pages yum -y update
#install platform ym -y install httpd
# copy the code to document : /var/www/html
#set any env variable for backend LB : BACKENDLB
#Apache is running on port 80
# ADD extracts and copy zip/tz files
# ADD will be able to download from url
FROM centos:7
MAINTAINER sraghva@yahoo.com
RUN yum -y update
RUN yum -y install httpd
#RUN useradd apache
#USER apache
#RUN mkdir /apps
#WORKDIR /apps
ADD code /var/www/html
ENV BACKENDLB=text
EXPOSE 80
CMD ["apachectl","-D","FOREGROUND"]
