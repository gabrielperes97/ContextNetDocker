FROM gabrielperes97/opensplice:6.7

RUN apt-get update && apt-get install -y wget

ADD ospl.xml $OSPL_HOME/etc/config/ospl.xml

WORKDIR /root

RUN wget https://bitbucket.org/endler/contextnet-dependencies/raw/master/br/pucrio/inf/lac/contextnet/2.7/contextnet-2.7.jar

CMD java -jar contextnet-2.7.jar 127.0.0.1 5500 ospl