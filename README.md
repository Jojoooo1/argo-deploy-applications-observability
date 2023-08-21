# Argo observability personal labs

## Observability applications

Available Applications:

| Applications  | DNS | Username  | Password | Links |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| Grafana | <https://grafana.local.com.br> | admin | password | <https://grafana.com/grafana/> |
| Prometheus | <https://prometheus.local.com.br> | | | <https://prometheus.io> |
| Alert-manager | <https://alertmanager.local.com.br> | | | <https://prometheus.io/docs/alerting/latest/alertmanager> |

## ArgoCD Folders organization

### Base

- **base/applications-observability**: Contains k8s observability applications

### Overlay

Environments folders that inherit from base folder. It uses [kustomize](https://github.com/kubernetes-sigs/kustomize) to allow environment based customization.
