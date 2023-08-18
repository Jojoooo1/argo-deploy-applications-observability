# Argo infra personal labs

## Observability applications

Available Applications:

- grafana: <http://grafan.local.com.br>
  - username: 'user', password: 'password'
- prometheus: <http://prometheu.local.com.br>
- alertmanager: <http://alertmanage.local.com.br>

## ArgoCD Folders organization

### Base

- **base/applications-observability**: Contains k8s observability applications

### Overlay

Environments folders that inherit from base folder. It uses [kustomize](https://github.com/kubernetes-sigs/kustomize) to allow environment based customization.
