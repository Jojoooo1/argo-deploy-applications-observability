# ArgoCD Observability labs

## Applications

| Applications  | DNS | Username  | Password | Links |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| Grafana | <https://grafana-local.cloud-diplomats.com> | admin | password | <https://grafana.com/grafana/> |
| Prometheus | <https://prometheus-local.cloud-diplomats.com> | | | <https://prometheus.io> |
| Alert-manager | <https://alertmanager-local.cloud-diplomats.com> | | | <https://prometheus.io/docs/alerting/latest/alertmanager> |

## Folders organization

### Applications

#### Base

- **grafana-dashboards-app**: Contains Grafana observability dashboards.
- **prometheus-rules-app**: Contains Prometheus Alerting Rules.

#### Overlay

Environments folders that inherit from base folder. It uses [kustomize](https://github.com/kubernetes-sigs/kustomize) to allow environment based customization.

### ArgoCD Applications

#### Base

- **base**: Contains ArgoCD Observability Applications

#### Overlay

Environments folders that inherit from base folder. It uses [kustomize](https://github.com/kubernetes-sigs/kustomize) to allow environment based customization.
