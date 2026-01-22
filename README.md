# K8s GitOps Demo

Demo GitOps repository for Lens Platform testing.

## Structure

```
.
├── namespaces/           # Namespace definitions
│   └── demo-app.yaml
├── apps/
│   ├── nginx/            # Nginx web server
│   │   ├── deployment.yaml
│   │   ├── service.yaml
│   │   └── configmap.yaml
│   └── api/              # Simple API server
│       ├── deployment.yaml
│       └── service.yaml
```

## Usage

Apply all manifests:

```bash
kubectl apply -f namespaces/
kubectl apply -f apps/nginx/
kubectl apply -f apps/api/
```

## Managed by

This repository is managed by Lens Platform AI agents for GitOps workflows.
