  GNU nano 4.8                                Dockerfile                                           
FROM ubuntu
RUN apt-get update \
   && apt-get install maven -y \
   && apt-get install git -y \
   && git clone https://github.com/yura40klg/42paas.git /var/app \
   && cd /var/app \
   && mvn clean && mvn install \
   && mkdir /var/share \
   && cp /var/app/target/App42PaaS-Java-MySQL-Sample-0.0.1-SNAPSHOT.war /var/share/app.war
CMD ["mvn"]

