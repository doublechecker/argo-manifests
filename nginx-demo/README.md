# Instructions
```bash
argocd proj create -f project.yaml
argocd app create -f application.yaml
```

This will create a argocd project (nginx-demo) and application (nginx) wich is installed from the helm-chart-repo source (https://kubernetes.github.io/) and the values.yaml is used to override a value (in this case the http port) wich comes from the git-repository source (https://github.com/doublechecker/argo-manifests) 