**Terraform execution**
terraform init -upgrade
terraform init
terraform plan
terraform apply
terraform destroy

**Create kubernerntes namespace**
 kubectl create namespace exercise

**Create deployment file**
kubectl create -f /path-to-deployment

https://hub.docker.com/layers/amulyakrishnan123/hello-world-excerise/latest/images/sha256-4f44b7713c5b2d18e37ca8fb550a751d6914ad859592338203b3ae39e7491cec?context=repo

with a username and password. A “config.json” file with an authorization token is created / updated in ~/.docker/config.json. The file can be opened and viewed. If we use a docker credentials store, instead of auth section. credstore details will be present.

kubectl create secret generic regcred — from-file=.dockerconfigjson=~/.docker/config.json — type = kubernetes.io/dockerconfigjson

kubectl apply -f service.yaml

kubectl get svc -n exercise

Look for the EXTERNAL-IP field of the hello-world-service. Once the external IP address is assigned, you can access your "Hello World" application using a web browser

