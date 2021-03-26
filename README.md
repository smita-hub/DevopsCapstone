# DevopsCapstone
My AWS Devops capstone project




kubectl set image deployment/flask-app flask-app=docker.io/smita0208/hello_flask_app:latest
kubectl rollout status -w deployment/flask-app

