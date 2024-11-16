# Demo ArgoCD <br>
### Handson : <br>
1.Create a git repo // sample <br>
2.Add Argo application configuration file // eg. argo-application.yaml <br>
3.Place kubernetes manifest files in it. <br>
4.Apply the argo application file :  <br>
  -kubectl apply -f manifests/argocd-application.yaml <br>
5.Check if sync is working :  <br>
  -kubectl get application -n argocd //status should update healthy <br>
6.Change replica settings at the runtime //observe that there is no change in cluster <br>
7.Change the replicas in the git repo //observe the auto update <br>
