# https://github.com/open-telemetry/opentelemetry-helm-charts/tree/main/charts/opentelemetry-collector

# Install helm repo
```
helm repo add opentelemetry https://open-telemetry.github.io/opentelemetry-helm-charts
helm repo update
```

# Get latest chart version
```
helm repo update && helm search repo opentelemetry/opentelemetry-collector
```

# Change version at Chart.yaml and then run
```
# Update chart dependencies
helm dependency update charts/opentelemetry-collector

# Build chart dependencies
helm dependency build charts/opentelemetry-collector
```