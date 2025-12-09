Helm installation and deployment

```
Install Helm
------------
apt update
apt install helm
sudo apt-get update
sudo apt-get install curl gpg apt-transport-https --yes
curl -fsSL https://packages.buildkite.com/helm-linux/helm-debian/gpgkey | gpg --dearmor | sudo tee /usr/share/keyrings/helm.gpg > /dev/null
echo "deb [signed-by=/usr/share/keyrings/helm.gpg] https://packages.buildkite.com/helm-linux/helm-debian/any/ any main" | sudo tee /etc/apt/sources.list.d/helm-stable-debian.list
sudo apt-get update
sudo apt-get install helm
helm version
helm repo list
helm version
helm repo list
helm repo add bitnami
sudo apt-get remove docker docker-engine docker.io containerd runc
sudo apt-get update
sudo apt-get install -y apt-transport-https ca-certificates curl gnupg-agent software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
sudo usermod -aG docker adminabdul
docker run hello-world
docker ps
  
KinD install
------------
sudo curl -L "https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl" -o /usr/local/bin/kubectl
sudo chmod +x /usr/local/bin/kubectl
kubectl version --client
sudo curl -Lo /usr/local/bin/kind https://kind.sigs.k8s.io/dl/v0.30.0/kind-linux-amd64
sudo chmod +x /usr/local/bin/kind
kind get clusters
kind create cluster
kubectl cluster-info --context kind-kind
kind get clusters
helm repo add bitnami https://charts.bitnami.com/bitnami
helm repo list
helm repo update
helm search repo bitnami
helm search repo bitnami | grep nginx
kubectl get pods
helm install nginxv1 bitnami/nginx
kubectl get pods
helm list
helm create nginx-chart
helm list charts
helm chats list
helm --help
helm show nginx-chart
helm show chart nginx-chart
ll
cd nginx-chart/
ll
cat values.yaml
ll
cd templates/
ll
cd ..
ll
cat Chart.yaml
vi Chart.yaml
cat Chart.yaml
ll
vim values.yaml
cd templates/
ll
vi deployment.yaml
vi service.yaml
vi ingress.yaml
ll
vi configmap.yaml
cd ..
ll
helm install my-nginx ./nginx-chart
cd nginx-chart/templates/
ll
vi serviceaccount.yaml
ll
vi serviceaccount.yaml
vi hpa.yaml
vi httproute.yaml
helm install my-nginx ./nginx-chart
cd ..
helm install my-nginx ./nginx-chart
cd nginx-chart/
ll
cd templates/
ll
rm NOTES.txt
cd -
helm install my-nginx ./nginx-chart
cd ..
helm install my-nginx ./nginx-chart
helm list
kubectl get pods
cd nginx-chart/
ll
cd ..
ll
cd nginx-chart/
ll
cd charts/
ll
ls -lart
cd ../..
helm package nginx-chart
ll
helm install my-nginx2 nginx-chart-0.1.0.tgz
helm list
cd nginx-chart
ll
```
