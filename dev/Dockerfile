FROM ubuntu
RUN apt-get update \
   && apt-get install maven -y \
   && apt-get install git -y \
   && git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git /var/boxfuse \
   && cd /var/boxfuse \
   && mvn package \
   && mkdir /var/share \
   && cp /var/boxfuse/target/*.war /var/share/
CMD ["mvn"]