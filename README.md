# k8s_cluster_in_docker


curl -s https://raw.githubusercontent.com/k3d-io/k3d/main/install.sh | bash


docker pull rancher/k3s:v1.31.5-k3s1

k3d cluster create mycluster --image rancher/k3s:v1.31.5-k3s1

curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"

chmod +x kubectl

sudo mv kubectl /usr/local/bin/

kubectl get pods

