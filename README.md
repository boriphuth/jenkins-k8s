# jenkins-k8s

$ docker build -t boriphuth/jenkins-k8s:lts .
$ docker push boriphuth/jenkins-k8s:lts

#สร้าง Jenkins บน Minikube
$ kubectl create -f jenkins-pvc.yml
$ kubectl create -f jenkins-deployment.yml
$ kubectl create -f jenkins-service.yml

$ kubectl get deployment
$ kubectl get service
$ kubectl get pvc

$ minikube service jenkins-k8s-service

$ kubectl create -f fabric8-rbac.yml

# Run

$ minikube service my-app-service


https://github.com/boriphuth/simple-spring-restful-app

# Reference
https://medium.com/@phayao/%E0%B8%AA%E0%B8%A3%E0%B9%89%E0%B8%B2%E0%B8%87-ci-cd-%E0%B8%94%E0%B9%89%E0%B8%A7%E0%B8%A2-jenkins-%E0%B8%9A%E0%B8%99-kubernetes-%E0%B9%81%E0%B8%9A%E0%B8%9A%E0%B8%87%E0%B9%88%E0%B8%B2%E0%B8%A2%E0%B9%86-fd4a1a496c46
