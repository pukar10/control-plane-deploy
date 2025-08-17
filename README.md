# control-plane-deploy
Control-plane repo utilizing ArgoCD App of apps to bootstrap the control-plane cluster for my homelab.

## Project

* `apps/` - 
* `manifests` - 

## Deployment

1. `kubectl create ns argocd`
2. `kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/v3.1.0/manifests/install.yaml`
3. `kubectl apply -n argocd -f apps/00-parent/control-plane.yaml`
4. Verify metalLB with `kubectl -n argocd get applications.argoproj.io`
