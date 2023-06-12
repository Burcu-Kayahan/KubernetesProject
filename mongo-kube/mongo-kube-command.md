 1  kubectl
    2  clear
    3  kubectl cluster-info
    4  kubeadm token create --print-join-command
    5  clear
    6  kubectl run mongo --image mongo:4 --env MONGO_INITDB_ROOT_USERNAME=admin --env MONGO_INITDB_ROOT_PASSWORD=password
    7  kubectl get po
    8  kubectl get po -o wide
    9  kubectl expose po mongo --port 27017 --type NodePort
   10  kubectl get svc
   11  kubectl get po mongo -o yaml 
   12  history
   13  kubectl api-resources
   14  kubectl get po,svc
   15  kubectl delete po mongo
   16  kubectl delete svc  mongo
   17  clear
   18  ls
   19  kubectl apply -f .
   20  history
   21  kubectl apply -f .
   22  kubectl get po,svc
   23  history