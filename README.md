# gen10-d-elk-202
es logstash kinaba

https://blog.csdn.net/qq_38899062/article/details/119325638

docker tag kibana:7.13.0 192.168.3.201:80/library/kibana:7.13.0
docker tag elasticsearch:7.13.0 192.168.3.201:80/library/elasticsearch:7.13.0
docker tag logstash:7.13.0 192.168.3.201:80/library/logstash:7.13.0
docker tag elastic/filebeat:7.13.0 192.168.3.201:80/library/elastic/filebeat:7.13.0

docker push 192.168.3.201:80/library/kibana:7.13.0
docker push 192.168.3.201:80/library/elasticsearch:7.13.0 &\
docker push 192.168.3.201:80/library/logstash:7.13.0 &\
docker push 192.168.3.201:80/library/elastic/filebeat:7.13.0