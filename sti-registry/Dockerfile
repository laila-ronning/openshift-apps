FROM skatt/java
ENV hostname localhost
ENV PORT_BASE 20000 
EXPOSE 20000 
ENV VERSION 1.2.1
ENV URL http://aurora.skead.no/nexus/service/local/repositories/releases/content/ske/registry/registry-leveransepakke/$VERSION/registry-leveransepakke-$VERSION-Leveransepakke.zip
ADD $URL /tmp/
USER root
RUN yum install -y unzip && \
  unzip -d /home/default /tmp/registry-leveransepakke-$VERSION-Leveransepakke.zip
USER default
WORKDIR /home/default/registry-leveransepakke-$VERSION/
ADD etc etc
ADD bin/start.sh bin/start.sh
CMD bin/start.sh

