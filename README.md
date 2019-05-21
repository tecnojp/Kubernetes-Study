# Basic Commands for my Kubernetes Study

Create resources using yml file.
kubectl create -f .\nginx-app.yml

Apply Updates after changing the yml file
kubectl apply -f .\nginx-app.yml --record=true

Show the progress of the Deployment
kubectl rollout status deployment my-nginx

Get the history of deployments
kubectl rollout history deployment

Start a Rollback of a Deployment for a previous revision
kubectl rollout undo deployment my-nginx --to-revision=