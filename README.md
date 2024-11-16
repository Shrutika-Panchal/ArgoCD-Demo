# Demo ArgoCD 
### Handson : 
1.Create a git repo // sample <br>
2.Add Argo application configuration file // eg. argo-application.yaml
3.Place kubernetes manifest files in it.
4.Apply the argo application file : 
  -kubectl apply -f manifests/argocd-application.yaml
5.Check if sync is working : 
  -kubectl get application -n argocd //status should update healthy
6.Change replica settings at the runtime //observe that there is no change in cluster
7.Change the replicas in the git repo //observe the auto update
