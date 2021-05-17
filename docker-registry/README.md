https://github.com/twuni/docker-registry.helm

Get ca secret :
kubectl get secrets -n docker-registry-ns tls-secret --output=jsonpath={.data.ca\\.crt} | base64 -d
