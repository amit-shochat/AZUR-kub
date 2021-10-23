# Dashboard app  

**To use this docker image you can clon the repo and built the dokcer image or load the docker image in this**

**Dockerfile stage**
<pre> 
#Choose the base image
FROM alpine:3.7 

#Force work ENV
WORKDIR /app

#COPY all file to container work dir
ADD ./app-count /app

#PORT 
EXPOSE 9001

#Environment variable
ENV PORT 9001

#RUN command for app 
CMD ["./counting-service"]
</pre>


to load this image you can use the command:
Example command to run:                                         
>docker load -i amitshochat66_app-count:1.0.0.tar

to build 
Example command to run:                                         
>docker build -t Dockerfile .
