# Devops-argocd
A part of cicd project
* Note: This repo is a part of cicd project, If you want to build full project go to [there](https://github.com/haquocdat543/devops-infra.git) first

### 1. Clone repo
```
git clone https://github.com/haquocdat543/devops-argocd.git
cd devops-argocd
```
### 2. Apply argo app
```
kubectl apply -f argocd.yaml
```
### 3. Check argocd result
### 4. Expose app to internet
```
kubectl patch svc myapp-service -n argocd -p '{"spec": {"type": "LoadBalancer"}}'
```
Result:
