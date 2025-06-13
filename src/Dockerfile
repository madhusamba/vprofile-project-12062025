# Use an official Tomcat base image
FROM tomcat:10.1-jdk17-temurin

# Remove default web apps (optional, keeps image clean)
RUN rm -rf /usr/local/tomcat/webapps/*

# Copy your WAR file to the Tomcat webapps directory
COPY target/*.war /usr/local/tomcat/webapps/ROOT.war

# Expose default Tomcat port
EXPOSE 8080

# Start Tomcat server
CMD ["catalina.sh", "run"]
