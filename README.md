# control-plane-deploy
Control-plane repo utilizing ArgoCD App of apps to bootstrap the control-plane cluster for my homelab.

## Project

* `apps/` - 
* `manifests` - 

## Deployment

1. Deploy [argocd-launch](https://github.com/pukar10/argocd-launch)
2. Deploy Parent control-plane app
   1. `kubectl apply -f template/control-plane.yaml`
