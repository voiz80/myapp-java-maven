# myapp-java-maven
### Deploy on k8 AWS

#### First we need created EKS on AWS

### On Jenkins server need to install and configure

- Install kubectl
- Install aws-iam-authenticator
- Create kubeconfig
    - .kube/config must be configured with AWS
- Add AWS credentials
- Adjust Jenkinsfile to configure EKS cluster deployment
