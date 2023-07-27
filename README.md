# Node_Prometheus

# Primeiros passos Promethes
# Curso Prometheus + Grafana

npm i

nodemon index.js

# Analise de requisições no browser:

http://localhost:3010/

http://localhost:3010/metrics

# Documents:

https://prometheus.io/docs/instrumenting/clientlibs/

>Nodejs

# Criando container para a folder prometheus 
<!-- docker run --name prometheus -d -p 9090:9090 -v "/Users/adalbertoramosribeiro/Desktop/Prometheus/Node_Prometheus/prometheus/prometheus.yml:/etc/prometheus/prometheus.yml" prom/prometheus -->

<!-- docker network create grafana-prometheus

docker pull prom/prometheus:latest -->

docker run --name my-prometheus --network grafana-prometheus --network-alias prometheus --publish 9090:9090 --volume ${pwd}/Users/adalbertoramosribeiro/Desktop/Prometheus/Node_Prometheus/prometheus/prometheus.yml:/etc/prometheus/prometheus.yml --detach prom/prometheus

# docker grafana

docker run --name grafana --network grafana-prometheus --network-alias grafana --publish 3001:3000 --detach grafana/grafana-oss:latest


## Grafana Docker:
docker run -d --name=grafana -p 3001:3000 grafana/grafana-enterprise

