docker build --build-arg JAR_FILE=target/config-service-0.0.6-SNAPSHOT.jar -t config-service .


docker push ghcr.io/codingkiddo/config-service:0.0.8-SNAPSHOT





kubectl apply -f k8s/deployment.yml

kubectl delete -f k8s/deployment.yml

kubectl logs deployment/config-service


  
  kubectl create -f dockerconfigjson.yaml
  
  kubectl delete -f dockerconfigjson.yaml