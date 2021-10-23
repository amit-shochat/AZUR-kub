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
