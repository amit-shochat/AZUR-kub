#Choose the base image
FROM alpine:3.7

#Force work ENV
WORKDIR /app

#COPY  all file to container work dir
ADD ./app-dashboard /app

#PORT
EXPOSE 9002

#Environment variable
ENV PORT 9002
ENV COUNTING_SERVICE_URL http://counting.service.consul:9001

#RUN command for app 
CMD ["./dashboard-service"]
