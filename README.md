# Helm Chart - Senhas App

Este repositório contém o Helm Chart para a aplicação **Senhas App** baseada em dois componentes principais: o serviço de backend que gerencia as senhas e o serviço de banco de dados Redis que armazena as informações temporárias e persistentes.

## Comandos Úteis

### Comandos para Instalar o Chart no Kubernetes

Para instalar o Helm Chart na sua instância do Kubernetes, execute o seguinte comando no diretório onde o chart está localizado:

```bash
helm install silmara-senhas ./

helm uninstall silmara-senhas

helm update silmara-senhas ./

helm update silmara-senhas ./

k get pods,svc,deploy

k port-forward svc/silmara-senhas-app 5000:5000  ---> Acessar via localhost:5000
