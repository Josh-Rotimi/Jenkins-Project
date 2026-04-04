# django-todo
A simple todo app built with django

![todo App](https://raw.githubusercontent.com/shreys7/django-todo/develop/staticfiles/todoApp.png)

## CICD Architecture [GitHub -> Jenkins -> k8s Manifests -> Argo CD -> k8s cluster]

![Screenshot 2023-02-01 at 2 48 06 PM](https://user-images.githubusercontent.com/43399466/216001659-74024e94-2c3c-4f1a-8e2e-3ef69b3a88ad.png)

sudo apt update
sudo apt install fontconfig openjdk-21-jre
sudo apt install jenkins
sudo apt install docker.io
sudo su
cat /var/...
sudo usermod -aG docker jenkins
sudo usermod -aG docker ubuntu
sudo systemctl restart jenkins
su - ubuntu
docker run hello-world
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube 
minikube start --driver=docker
df -h
git clone https://github.com/Josh-Rotimi/Jenkins-Project.git
cd Jenkins-Project/python-jenkins-argocd-k8s/deploy
sudo snap install kubectl --classic
kubectl apply -f deploy.yaml
kubectl apply -f service.yaml
kubectl get svc
minikube service todo-service
kubectl port-forward --address 0.0.0.0 service/todo-service 31000:80
