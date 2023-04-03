FROM tomcat:8-jre11
LABEL "Project"="Vprofile"
LABEL "Author"="Chaitanya"
# to remove any default application
RUN rm -rf /usr/local/tomcat/webapps/*
# copy war file using COPY
COPY target/vprofile-v2.war /usr/local/tomcat/webapps/ROOT.war
# Setting PORT
EXPOSE 8080
CMD ["catalina.sh","run"]
# set-up work directory
WORKDIR /usr/local/tomcat/
VOLUME /usr/local/tomcat/webapps
