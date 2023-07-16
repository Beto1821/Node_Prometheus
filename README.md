# Node_Prometheus

# Primeiros passos Promethes
# Curso Prometheus + Grafana

npm i

nodemon index.js

# Analise de requisições no browser:

http://localhost:3000/

http://localhost:3000/metrics

# Documents:

https://prometheus.io/docs/instrumenting/clientlibs/

>Nodejs

# Criando container para a folder prometheus 
docker run --name prometheus --rm -d -p 9090:9090 -v "/Users/adalbertoramosribeiro/Desktop/Prometheus/Node_Prometheus/prometheus/prometheus.yml:/etc/prometheus/prometheus.yml" prom/prometheus

