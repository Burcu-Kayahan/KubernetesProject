 18  kubectl delete -f .
   19  kubectl apply -f .
   20  kubectl get ingress my-ingress
   21  kubectl describe ingress my-ingress
   22  kubectl get svc
   23  kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.7.1/deploy/static/provider/cloud/deploy.yaml
   24  kubectl get svc
   25  kubectl get ingress
   26  kubectl get svc -A
   27  history