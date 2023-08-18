# Argo infra personal labs

## Network

Network with wifi router configuration can block some port and leave the k3s without stable communication. If you want to make sure there is none, try using your 4G network.

## Getting Started

Create local cluster with [k3s](https://k3s.io/):

```bash
cd overlays/local/_scripts
./start.sh
```

### Argocd dashboard

- [http://argo-local.jonathan.com.br](http://argo-local.jonathan.com.br/)
    - login: admin password: see the logs

### Infra applications

You can then use the following applications after syncing the corresponding argo apps:

- keycloak: <http://identity-local.jonathan.com.br/admin/master/console>
  - username: 'admin', password: 'password'
- rabbitmq: <http://rabbitmq-local.jonathan.com.br>
  - username: 'user', password: 'bitnami'

### Observability applications

You can then use the following applications after syncing the corresponding argo apps:

- grafana: <http://grafana-local.jonathan.com.br>
  - username: 'user', password: 'password'
- prometheus: <http://prometheus-local.jonathan.com.br>
- alertmanager: <http://alertmanager-local.jonathan.com.br>

## ArgoCD Folders organization

### Base

- **base/applications-observability**: Contains k8s observability applications

- **base/applications-infra**: Contains k8s infra applications

### Overlay

Environments folders that inherit from base folder. It uses [kustomize](https://github.com/kubernetes-sigs/kustomize) to allow environment based customization.
