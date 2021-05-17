# PaC

**P**latform **a**s **C**ode

## Deploy Services

``` bash
docker-compose run kubectl apply -f <service_name>

# Exemple
docker-compose run kubectl apply -f docker-registry
``` 

## Remove Services

``` bash
docker-compose run kubectl delete -f <service_name>

# Exemple
docker-compose run kubectl delete -f docker-registry
``` 

## Services list

Name            | Path                               | src        | Description            
:--------:      |:---                                |:---        | :---
Operator        | cluster-monitoring/manifests/setup | carlosedp  | Install operator <TBD>
Monitoring      | cluster-monitoring/manifests       | carlosedp  | Install monitoring tools (alerting, exporter, prometheus,...)
pihole          | pihole                             | see readme | pihole is a local DNS and ads blocker
metallb         | metallb                            |            | kubernetes load balancer
metallb-test    | metallb/test                       |            | Test metallb deployement
docker-registry | docker-registry                    |            | Private Docker registry  



