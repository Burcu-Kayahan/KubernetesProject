 Id CommandLine
  -- -----------
   1 try { . "c:\Users\Burcu\AppData\Local\Programs\Microsoft VS Code\resources\app\out\vs\workbench\contrib\... 
   2 kubectl get po
   3 minikube start
   4 kubectl get po
   5 kubectl create deployment my-deploy --image nginx --replicas 3
   6 kubectl describe deployment my-deploy
   7 kubectl get rp
   8 kubectl get deploy
   9 kubectl delete deploy my-deploy
  10 kubectl create deployment my-deploy --image=nginx  --replicas=3
  11 kubectl get deploy
  12 kubectl get rp
  13 kubectl get pods
  14 kubectl get pod -o wide
  15 kubectl describe pod my-deploy-85f646f9bf-5vfhb
  16 kubectl exec -it my-deploy-85f646f9bf-5vfhb -- ls
  17 kubectl exec -it my-deploy-85f646f9bf-5vfhb -- bash
  18 kubectl get rs,deploy
  19 kubectl scale deploy nginx-deployment --replicas=5
  20 kubectl scale deploy my-deploy  --replicas=5
  21 kubectl get deploy
  22 kubectl delete deploy my-deploy
  23 kubectl apply -f devops-deploy.yaml
  24 cd .\deployment-lesson\
  25 kubectl apply -f devops-deploy.yaml
  26 kubectl get deploy,rs,po -l app=container-info
  27 kubectl rollout history deploy devops-deploy
  28 kubectl rollout history deploy devops-deploy --revision=1
  29 kubectl set image deploy devops-deploy container-info=gluobe/container-info:blue
  30 kubectl rollout history deploy devops-deploy
  31 kubectl rollout history deploy devops-deploy --revision=2
  32 kubectl get deploy,rs,po -l app=container-info
  33 kubectl edit deploy/devops-deploy
  34 kubectl rollout history deploy devops-deploy
  35 kubectl rollout history deploy devops-deploy --revision=3
  36 kubectl get deploy,rs,po -l app=container-info
  37 kubectl rollout undo deploy devops-deploy --to-revision=1
  38 kubectl rollout history deploy devops-deploy
  39 kubectl rollout history deploy devops-deploy --revision=1
  40 kubectl get deploy,rs,po -l app=container-info -o wide
  41 kubectl rollout history deploy devops-deploy --revision=1
  42 kubectl rollout history deploy devops-deploy --revision=2
  43 kubectl rollout history deploy devops-deploy --revision=4
  44 kubectl get ns
  45 kubectl get po -n kube-system
  46 kubectl get po -n kube-public
  47 kubectl describe po kube-apiserver-minikube -n kube-system
  48 kubectl create ns devops-namespace
  49 kubectl get ns
  50 kubectl create deployment devops-ns --image=nginx -n=devops-namespace
  51 kubectl create deployment default-ns --image=nginx
  52 kubectl get ns
  53 kubectl get deploy
  54 kubectl get deploy -n devops-namespace
  55 kubectl get all -A
  56 kubectl create deployment my-deploy --image nginx --replicas 3 --dry-run client -o yaml
  57 kubectl create deployment my-deploy --image nginx --replicas 3 --dry-run=client -o yaml
  58 kubectl create deployment my-deploy --image nginx --replicas 3
  59 kubectl get deploy
  60 kubectl expose deployment my-deploy --port 80 --dry-run=client -o yaml
  61 kubectl expose deployment my-deploy --port 80
  62 kubectl get service
  63 kubectl get deploy --show-labels
  64 kubectl get svc --show-labels
  65 kubectl describe svc my-deploy
  66 kubectl get po -o wide
  67 kubectl get svc
  68 kubectl run kutu --image busybox -- command sleep 3600
  69 kubectl exec -it kutu -- sh
  70 kubectl get po
  71 kubectl delete pod kutu
  72 kubectl run kutu --image busybox --command sleep 3600
  73 kubectl exec -it kutu -- sh