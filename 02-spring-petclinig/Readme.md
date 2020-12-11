# Spring Petclinic Configuration Repository

ytt -f k8s -f values.yaml | kapp deploy -n petclinic -a petclinic -y -f -  

kubectl get svc -n petclinic spring-petclinic -o jsonpath="{.status.loadBalancer.ingress[0].hostname}"


