# Install MariaDB
kubectl create ns petclinic  
helm repo add tac https://charts.trials.tac.bitnami.com/demo  
helm install -f mariadb.yaml petclinic-db tac/mariadb -n petclinic  
kubectl get po -n petclinic -w  
