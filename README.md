# cloud-native-jira
jira installation on docker, kubernetes and openshift

### jira deployment on kubernetes
create persistent volume and claim
```
kubectl apply -f https://raw.githubusercontent.com/koseburak/cloud-native-jira/master/k8s/jira-persistentvolume.yaml
```
create node port service
```
kubectl apply -f https://raw.githubusercontent.com/koseburak/cloud-native-jira/master/k8s/jira-service.yaml
```
create config map
```
kubectl apply -f https://raw.githubusercontent.com/koseburak/cloud-native-jira/master/k8s/jira-configmap.yaml
```
create deployment
```
kubectl apply -f https://raw.githubusercontent.com/koseburak/cloud-native-jira/master/k8s/jira-deployment.yaml
```
