# Install MariaDB
kubectl create ns petclinic  
helm install -f mariadb.yaml petclinic-db tac/mariadb -n petclinic  
kubectl get po -n petclinic -w  
