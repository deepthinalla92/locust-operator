# locust-operator
kubernetes operator to deploy locust in distributed mode

## Steps
1. go mod init github.com/deepthinalla92/locust-operator
2. kubebuilder init --domain leftbin.com --license apache2 --owner "Deepthi Nalla"
3. kubebuilder create api --group locust --version v1alpha1 --kind LocustCluster
4. make docker-build docker-push IMG=deepthinalla/locust-operator:0.0.1
5. make deploy IMG=deepthinalla/locust-operator:0.0.1
