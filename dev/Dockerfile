FROM ubuntu
RUN apt-get update \
   && apt-get install maven -y \
   && apt-get install git -y \
   && git clone https://https://github.com/shephertz/App42PaaS-Java-MySQL-Sample.git /var/app \
   && cd /var/app \
   && mvn package \
   && mkdir /var/share \
   && cp /var/app/target/App42PaaS-Java-MySQL-Sample.0.0.1-SNAPSHOT.war /var/share/app.war
CMD ["mvn"]
