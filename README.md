# otel-monitoring-stack

## Install docker desktop
https://www.docker.com/products/docker-desktop/

## Enable start docker desktop and enable kubernetes
![k8s location](https://github.com/jonnywony/monitoring-otel-stack/blob/main/k8s-location.png?raw=true)

## Install kubectl
brew install kubectl

## Install helm templating tools
brew install helmfile <br />
brew install helm <br />
https://github.com/databus23/helm-diff <br />
helm plugin install https://github.com/databus23/helm-diff

## Run helmfile apply
helmfile apply

## Run port forward to expose the frontend
kubectl port-forward svc/otel-frontendproxy 8080:8080

## Run port forward to expose the open telemetry collector
kubectl port-forward svc/otel-otelcol 4318:4318
