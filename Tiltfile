# Build
docker_build ('config-service', '.')
)

# Deploy
k8s_yaml(['k8s/deployment.yml'])

# Manage
k8s_resource('config-service', port_forwards=['8888'])