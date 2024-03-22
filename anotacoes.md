**Comandos:**

*Verificar pods:*
kubectl get pods

*Criar pod:*
kubectl run (nome do pod) --image=(imagem do pod)

*Deletar pod:*
kubectl delete pod (nome)
*Para pods declarativos:
kubectl delete -f (PATH do pod)

*Descrição do pod*
kubectl describe pod (nome do pod)

*Editar pod*
kubectl edit pod (nome do pod)

*Criar de maneira declarativa*
kubectl apply -f (PATH)

*Executar de maneira interativa*
kubectl exec -it (nome) -- (comando)