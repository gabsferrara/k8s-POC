POC k8s.


lembretes:

utlizado fortio para stress
tambem tem a k6s p stress

alguns comandos:

$ kubectl config use-context ...
$ kubectl port-forward service/goserver-service 8080:8080
$ kubectl apply -f k8s/service.yaml //f de file
$ kubectl get
$ kubectl delete
$ kubectl rollout history deployment ... --to-revesion ...
$ kubectl proxy --port=...
$ kubectl run -it fortio --rm --image=fortio/fortio -- load -qps 800 -t 120s -c 70 "http://goserver-service/healthz"
$ kubectl get storageclass
$ kubectl get pods -n=.... // n de namespace
$ kubectl config view
$ kubectl config current-context
$ kubectl config set-context NAMECONTEXT --namespace=xxx --cluster=NAMECLUSTER --user=User
$ kubectl api-resources


https://github.com/kubernetes-sigs/metrics-server

https://github.com/fortio/fortio

