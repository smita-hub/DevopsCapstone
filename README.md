# DevopsCapstone
My AWS Devops capstone project

eksctl create cluster --name devops-capstone --region us-west-2 --fargate

eksctl create nodegroup --cluster devops-capstone --node-type t3.medium --nodes 1 --ssh-access id_rsa.pub

aws eks --region us-west-2 update-kubeconfig --name devops-capstone --role-arn arn:aws:iam::765181591880:role/UdacityFlaskDeployCBKubectlRole

Access key ID

AKIA3EKDAQFEDSJ4YO4C

Secret access key

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

--ssh-public-key id_rsa.pub

aws iam create-role --role-name UdacityFlaskDeployCBKubectlRole --assume-role-policy-document file://trust.json --ssh-public-key id_rsa.pub --output text --query 'Role.Arn'