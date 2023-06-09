 31  kubectl apply -f secret.yaml
   32  kubectl get secret
   33  kubectl describe mysecret
   34  kubectl describe secret mysecret
   35  kubectl get secret mysecret -o yaml
   36  kubectl create secret generic mysecret2 --from-literal=db_server=db.example.com --from-literal=db_username=admin --from-literal=db_password=P@ssw0rd!
   37  kubectl get secrets
   38  kubectl describe secret mysecret2
   39  kubectl get secret mysecret2 -o yaml
   40  kubectl get secrets
   41  echo  'db.example.com' > server.txt
   42  cat server.txt
   43  echo 'admin' > username.txt
   44  cat username.txt
   45  echo 'P@ssw0rd!'  > password.txt
   46  cat password.txt
   47  kubectl create secret generic mysecret3 --from-file=db_server=server.txt --from-file=db_username=username.txt --from-file=db_password=password.txt
   48  kubectl get secrets
   49  clear
   50  kubectl create secret generic mysecret4 --from-file=secretconfig.json
   51  kubectl get secrets
   52  kubectl get secret secret4 -o yaml
   53  kubectl get secret mysecret4 -o yaml
   54  kubectl get secret mysecret -o yaml
   55  kubectl apply -f secret-env-pod.yaml
   56  kubectl get po
   57  kubectl exec -it secretpovolume -- sh
   58  kubectl exec -it secretpovolume -- bash
   59  kubectl exec -it secretpodvolume -- bash
   60  clear