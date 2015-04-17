FROM centos:7
MAINTAINER laila.ronning@skatteetaten.no

RUN yum update
RUN yum install -y java-1.7.0-openjdk
RUN yum clean all

#ADD registry-leveransepakke-1.1.38 /u01/java-apps/OPPSLAGSTJENESTE-UTV-app/registry-leveransepakke-1.1.38
#RUN cd /u01/java-apps/OPPSLAGSTJENESTE-UTV-app && ln -s registry-leveransepakke-1.1.38 current
#ADD registry.properties /u01/java-apps/OPPSLAGSTJENESTE-UTV-app/current/etc/
#ADD registry-env.properties /u01/java-apps/OPPSLAGSTJENESTE-UTV-app/current/etc/
#WORKDIR /u01/java-apps/OPPSLAGSTJENESTE-UTV-app/current
#EXPOSE 20000:20000
#CMD ./bin/start.sh

#ENTRYPOINT ["/registry"]
