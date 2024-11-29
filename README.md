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

k port-forward svc/silmara-senhas-app 5000:5000

helm lint silmara-senhas

helm template silmara-senhas-chart

helm package charts/silmara-senhas-chart

helm repo index --url https://github.com/silmarasilva/helm-chart-senhas-app.git .

No github > repositório > settings > page ---> definir a branch (root)

Vai aparecer essa msg até que sua página esteja pronta: "Your GitHub Pages site is currently being built from the main branch"

helm repo index -url  <link gerado no passo acima pelo github>

Commit com as alteracoes.

helm repo add <repo name> <link do seu chart>

helm repo list 

helm search repo <nome do seu chart>

helm install <chart senha> <nome atribuido ao repo> 

helm show all meu-novo-repos/silmara-senhas




















