# myapp-java-maven
### Deploy on k8 AWS

#### First we need created EKS on AWS
- Example:
```
eksctl create cluster \
--name demo-cluster \
--version 1.25 \
--region eu-central-1 \
--nodegroup-name demo-nodes \
--node-type t2.micro \
--nodes 2 \
--nodes-min 1 \
--nodes-max 3
```

### On Jenkins server need to install and configure

- Install kubectl
- Install aws-iam-authenticator
- Create kubeconfig
    - .kube/config must be configured with AWS
- Add AWS credentials
- Adjust Jenkinsfile to configure EKS cluster deployment
