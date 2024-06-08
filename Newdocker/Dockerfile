#Use the official Centos Apache HTTP server image
FROM centos/httpd

#Download and unzip the web content
#ADD https://www.free-css.com/assets/files/free-css-templates/download/page254/photogenic.zip /var/www/html
WORKDIR /var/www/html
RUN apt install -y unzip && unzip /var/www/html/photogenic.zip && rm /var/www/html/photogenic.zip

#Expose Port 80 for HTTP
EXPOSE 80

#start apache http server
CMD ["httpd", "-D", "FOREGROUND"] 
