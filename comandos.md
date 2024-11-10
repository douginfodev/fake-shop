## Kubernet Comandos

## Verificar os nos existentes
kubectl get nodes

### Verificar os pods
kubectl get pods

### verificar todos os pods
kubectl get all
kubectl get svc

### Executar um arquivo
kubectl apply -f nomedoarquivo.yaml>

### Pegar a senha do Grafana
kubectl get secret --namespace default grafana -o jsonpath="{.data.admin-password}" | base64 --decode ; echo