# ArgoCD example

## Quick start

To install latest argocd version use **./init/install-argo.sh**.


## Example

There are example scripts in ./init/ directory showing how to add automaticaly applications from git structure, like is defined here.
```
# define application sets for project developer / infra
├── appset-developer.yaml
├── appset-infra.yaml
# define argocd ingress (using nginx-ingress)
├── ingress.yaml
├── install-argo.sh
# define projects for project developer / infra applications
├── project-developers.yaml 
└── project-infra.yaml
```

## Structure and workflow




## How to contribute


```bash
# Compare local state with argo deployment
argocd app diff argocd/example-app-nginx-example --local ./argo-apps/example-app/nginx-example

```