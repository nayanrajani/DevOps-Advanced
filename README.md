# DevOps-Advanced

- DevOps-Advanced
  - The training is intended to fill the skill gap in Kubernetes-related technology/tools and will cover AWS EKS, Helm, Istio, ELK, Prometheus, Grafana, and ArgoCD, along with hands-on.
  - Changes added.

- Validate

  - You can validate the k8s access to the fargate cluster as below
    - add the secret key and access key in $HOME/.aws/credentials file under a given profile (ex. below)

  - Run the command
    - aws eks update-kubeconfig --region ap-south-1 --name EKS-ExternalTraining-Account2 --profile k8s-training
    - *Use name as EKS-ExternalTraining-Account1  for people specified with training account 1

  - Connect to vpn and run the below command
    - kubectl get pods -n kube-system

- Introduction to K8S

  - bogman by google