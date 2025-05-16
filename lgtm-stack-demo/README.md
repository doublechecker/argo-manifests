# Instrctions
```bash
argocd proj create -f project.yaml
argocd app create -f grafana/application.yaml
argocd app create -f loki/application.yaml
```

This will create a argocd application from an custom helm-chart (https://github.com/doublechecker/argo-manifests, /loki-helm-chart/Chart.yaml) in the default project (default).
