# ELK
Setup ELK environment


To setup the ELK environment with Docker and docker-compose, I used 3 images with same version : elasticsearch, logstash and kibana (version 8.2.3)

On the ELK repository, we have 3 differents folders (elasticsearch, logstash and kibana) containing each the service configuration :
* elasticsearch : contains configuration file elasticsearch.yml to configure all necessary informations like number of nodes, enable security, certificates locations ... This application run on port 9200
* logstash : contains configuration files (config for lostash configuration, pipeline for reading logs and send to elasticsearch [in our, we read from file]) and logs contains log files). This application run on port 5000
* kibana : contains configuration file kibana.yml to configure all necessary informations for kibana

## We use docker-compose :

* Define all services to setup ELK environment (elasticsearch, logstash and kibana)
* Build and run all thoses services

