# DevOps-Advanced

- https://github.com/amitvashisttech/kubernetes-eks-bs-28-Feb-2024
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

- Commands

  - kubectl api-resources
  - kubectl config set-context --current --namespace=nr-1-ns
  - echo d2FsbG1hcnQ= | base64 --decode
  - echo nayan.rajani@blazeclan.com | base64
    - bmF5YW4ucmFqYW5pQGJsYXplY2xhbi5jb20K 
  - echo N@pass123 | base64
    - TkBwYXNzMTIzCg==
  - kubectl exec -it nayan-deploy-6d8965c6fb-bldrs -- sh
  - kubectl create secret generic nayan-secret --from-file=username.txt
  - printenv
  - argocd account update-password \
  --current-password # current password \
  --new-password # new password
  - argocd.exe login aca87ca139d9a424a9783bc0610aa0e5-1304525760.ap-south-1.elb.amazonaws.com --insecure
  - argocd repo list
  - argocd repo add https://gitlab.com/nayan98/spacex-netflix.git --username nayan98 --password secret --insecure-skip-server-verification
  - $ kubectl get pods -A | grep kibana
  - $ kubectl delete pv --all -n spacex-efk