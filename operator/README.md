# Operator

Helm chart for Go based operators to use instead of default kustomize

> in this project we aimed to provide a helm chart to use instead of default `Kustomize` as deployment strategy when developing operators.
>
> **_NOTE:_** in this way, you don't have to generate rbac and webhooks automatically by `controller-gen` tool and you have to modify the values.yaml file based on your needs, you only need `controller-gen` tool to generate the CRDs based on what you have defined in your api directory.

Take a look at [caas-operator](https://github.com/mohammadne/caas-operator) project to get an insight for how using this chart.

> **_NOTE:_** with this deployment approach you normally need to change the default Makefile and specify `rbac` and `webhook` within the values of the chart (normally defined in make manifests).
