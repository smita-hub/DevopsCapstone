# DevopsCapstone
My AWS Devops capstone project

<<<<<<< HEAD



kubectl set image deployment/flask-app flask-app=docker.io/smita0208/hello_flask_app:latest
kubectl rollout status -w deployment/flask-app

=======
eksctl create cluster --name devops-capstone --region us-west-2 --fargate

eksctl create nodegroup --cluster devops-capstone --node-type t3.medium --nodes 1 --ssh-access id_rsa.pub

aws eks --region us-west-2 update-kubeconfig --name devops-capstone --role-arn arn:aws:iam::765181591880:role/UdacityFlaskDeployCBKubectlRole

xxx

--ssh-public-key id_rsa.pub

aws iam create-role --role-name UdacityFlaskDeployCBKubectlRole --assume-role-policy-document file://trust.json --ssh-public-key id_rsa.pub --output text --query 'Role.Arn'
>>>>>>> 250146fcbe0a61b4efd4fb130d2b7eb775614d52
