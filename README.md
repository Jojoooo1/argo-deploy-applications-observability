# ArgoCD Observability labs

## Apps

| Applications  | DNS | Username  | Password | Links |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| Grafana | <https://grafana-local.cloud-diplomats.com> | admin | password | <https://grafana.com/grafana/> |
| Prometheus | <https://prometheus-local.cloud-diplomats.com> | | | <https://prometheus.io> |
| Alert-manager | <https://alertmanager-local.cloud-diplomats.com> | | | <https://prometheus.io/docs/alerting/latest/alertmanager> |

## Folders organization

### Applications

#### applications/base

- **grafana-dashboards-app**: Grafana dashboards.
- **prometheus-rules-app**: Prometheus Alerting Rules.

#### applications/overlay

Environments folders that inherit from base folder. It uses [kustomize](https://github.com/kubernetes-sigs/kustomize) to allow environment based customization.

### ArgoCD Applications

#### argo-app/base

- **base**: ArgoCD Applications

#### argo-app/overlay

Environments folders that inherit from base folder. It uses [kustomize](https://github.com/kubernetes-sigs/kustomize) to allow environment based customization.
