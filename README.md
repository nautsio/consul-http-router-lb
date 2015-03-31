# Consul-template haproxy image

Basic image of the HA Proxy for consul-http-router. 

## How to use
```
docker run -d -p 80:80 cargonauts/consul-haproxy -consul consul.service.consul:8500 -template /haproxy.ctmpl:/etc/haproxy/haproxy.cfg:service haproxy restart
```
