# Info
In order to use the argo-cd-application-manifest, it needs to be in a repo that is accessible by the argocd-server. This can be a private repo, but you need to make sure that the argocd-server has access to it. You can do this by creating a secret with the credentials for the repo and then adding it to the argocd-server deployment.

For now, we can just use the cli command to create an application.

# Loki
Manifest: helm-loki.yaml
Command:
```bash
argocd app create loki \
  --repo https://grafana.github.io/helm-charts \
  --helm-chart loki \
  --revision 6.29.0 \
  --dest-namespace monitoring \
  --dest-server https://kubernetes.default.svc \
  --project default \
  --values ./values.yaml
  --insecure
```
