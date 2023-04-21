FROM almalinux
RUN yum install nginx -y 
# when this image is created, below command will not run. When this image is used as base image while creating 
# another image, then it will be executed 
ONBUILD ADD simple.txt /tmp/ 