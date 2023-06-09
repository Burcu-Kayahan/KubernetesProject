61  kubectl get po
   62  kubectl exec -it secretpodenv -- printenv
   63  kubectl exec -it secretpodenvall -- printenv
   64  kubectl apply -f config-map.yaml
   65  kubectl get cm
   66  kubectl get cm kube-root-ca.crt -o wide
   67  kubectl get cm kube-root-ca.crt -o yaml
   68  kubectl apply -f pod-env-var.yaml
   69  kubectl get po
   70  kubectl exec -it pod-env-var -- env
   71  kubectl delete -f .