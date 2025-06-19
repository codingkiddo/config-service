docker build --build-arg JAR_FILE=target/config-service-0.0.6-SNAPSHOT.jar -t config-service .


docker push ghcr.io/codingkiddo/config-service:0.0.8-SNAPSHOT




https://dev.to/asizikov/using-github-container-registry-with-kubernetes-38fb

echo -n "codingkiddo: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" | base64

Y29kaW5na2lkZG86Z2hwX1ZDNmdjQ0prU0FTT01jRjhiOHZqVjJ2cWc1V0twVzNVNHNWRQ==


echo -n  '{"auths":{"ghcr.io":{"auth":"Y29kaW5na2lkZG86Z2hwX1ZDNmdjQ0prU0FTT01jRjhiOHZqVjJ2cWc1V0twVzNVNHNWRQ=="}}}' | base64



kind: Secret
type: kubernetes.io/dockerconfigjson
apiVersion: v1
metadata:
  name: dockerconfigjson-github-com
  labels:
    app: app-name
data:
  .dockerconfigjson: eyJhdXRocyI6eyJnaGNyLmlvIjp7ImF1dGgiOiJZMjlrYVc1bmEybGtaRzg2WjJod1gxWkRObWRqUTBwclUwRlRUMDFqUmpoaU9IWnFWakoyY1djMVYwdHdWek5WTkhOV1JRPT0ifX19
  
  
  