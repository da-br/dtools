It is assumed docker and minikube is installed on your machine 

## Getting started

### Prerequisites

> for local development
> 1. mkcert


### Minikube addons

```bash
minikube addons enable ingress
```

## VaultWarden

create a namespace

```bash
kubectl create namespace vaultwarden
```

> for local development
> ```bash
> cd vaultwarden/base
> mkcert -install
> mkcert -cert-file cert.pem -key-file key.pem localhost
> ```

```bash
kubectl apply -k overlays/minikube
```
