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

*Histórico dos deployments*
kubectl rollout history (tipo) (nome)
// deployments permitem o controle de versionamento de imagens e pods

*Mudar valor da chave do history*
kubectl annotate (tipo) (nome) (chave)=(valor)
ex:
kubectl annotate deployment nginx-deployment kubernetes.io/change-cause="exemplo"

*Rollback*
kubectl rollout undo (tipo) (nome) --to-revision(versão)
ex:
kubectl rollout undo deployment nginx-deployment --to-revision=3