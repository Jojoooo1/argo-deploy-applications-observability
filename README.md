# Argo infra personal labs

## Observability applications

You can then use the following applications after syncing the corresponding argo apps:

- grafana: <http://grafana-local.jonathan.com.br>
  - username: 'user', password: 'password'
- prometheus: <http://prometheus-local.jonathan.com.br>
- alertmanager: <http://alertmanager-local.jonathan.com.br>

## ArgoCD Folders organization

### Base

- **base/applications-observability**: Contains k8s observability applications

### Overlay

Environments folders that inherit from base folder. It uses [kustomize](https://github.com/kubernetes-sigs/kustomize) to allow environment based customization.
