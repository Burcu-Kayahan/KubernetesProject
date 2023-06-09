
  Id CommandLine
  -- -----------
   1 try { . "c:\Users\Burcu\AppData\Local\Programs\Microsoft VS Code\resources\app\out\vs\workbench\contrib\term... 
   2 kubectl cluster-info
   3 kubectl cluster-info dump
   4 docker ps
   5 kind get nodes
   6 minikube ip
   7 minikube start
   8 minikube ip
   9 kubectl get node -o yaml
  10 kubectl get node -L os=linux
  11 kubectl get pod
  12 kubectl run mypod --image=busybox --command sleep 3600
  13 kubectl get po
  14 kubectl get po mypod -o yaml
  15 kubectl apply -f mypod.yaml
  16 kubectl get po
  17 kubectl describe po mypod.yaml
  18 kubectl describe po
  19 kubectl describe po benim
  20 kubectl describe po mypod2
  21 kubectl get po
  22 kubectl exec -it mypod -- sh
  23 kubectl get po
  24 kubectl apply -f double.yaml
  25 kubectl get po
  26 kubectl describe pod ikiz
  27 kubectl get po
  28 kubectl logs ikiz -c kutu1
  29 kubectl logs ikiz -c nginx
  30 kubectl get nodes -o wide
  31 curl 192.168.49.2
  32 kubectl get all
  33 kubectl create deploy mydeploy --image=nginx --replicas=3
  34 kubectl get po
  35 kubectl get rs
  36 kubectl get deploy
  37 kubectl scale deploy mydeploy --replicas=6
  38 kubectl scale rs mydeploy --replicas=2
  39 kubectl get deploy mydeploy -o yaml
  40 kubectl edit deploy mydeploy
