You can create Applications in ArgoCD in different ways.


# As Helm Chart

## In UI
"New App" -> Fill out Application and Project Name -> In "Source" select "Helm" -> Fill out the helm-repo URL, the chart-name and the chart-version -> Fill out the destination cluster and namespace.

You can also provide values in the text-field as yaml.

## In CLI
TODO


# As Application-Definition (via Git-Repository)

## In UI
TODO

## In CLI
"New App" -> Fill out Application and Project Name -> In "Source" select "Git" -> Fill out the git-repo URL (e.G. the example-repo "argo-manifests") and the path to the application.yaml file ("loki/via_application_def") -> Fill out the destination cluster and namespace.
