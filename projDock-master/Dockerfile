FROM hshar/tomcat1

RUN cd /usr/local/tomcat && \
    git clone https://github.com/hshar/test123.git && \
    cd test123 && \
    mvn install
RUN cd /usr/local/tomcat/test123 && \
    mv ./target/notificationapp-1.war .

RUN cd /usr/local/tomcat && \
    cp ./test123/notificationapp-1.war /usr/local/tomcat/webapps/
