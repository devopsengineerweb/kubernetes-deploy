LabRoleEKS
 -AmazonEKSClusterPolicy
 -AmazonEKSServicePolicy

aws eks create-cluster --name lab-kube --role-arn arn:aws:iam::706053428606:role/LabRoleEKS --resources-vpc-config subnetIds=subnet-065ddfd8c44ce63f9,subnet-0aefffc076d6ebde4,securityGroupIds=sg-0c3403d010cebd9a6

aws eks list-clusters

aws eks describe-cluster --name lab-kube

aws eks update-kubeconfig --name lab-kube

kubectl get svc

kubectl version


VPC
https://amazon-eks.s3-us-west-2.amazonaws.com/cloudformation/2018-12-10/amazon-eks-vpc-sample.yaml

Nodes
https://amazon-eks.s3-us-west-2.amazonaws.com/cloudformation/2018-12-10/amazon-eks-nodegroup.yaml