# Comandos

### Criar imagem docker
docker build -t fabricioje/hello-go .
docker run --rm -p 80:80 fabricioje/hello-go
docker push fabricioje/hello-go

### Criar um cluster
kind create cluster

### Verificar todos nodes rodando
kubectl get nodes 

### Verificar todos os clusters ativos
kind get clusters

### Deletar um cluster
kind delete clusters {nome_kuster}

### Criar cluster com arquivo yaml
kind create cluster --config=k8s.kind.yaml --name=helloword
* doc: https://kind.sigs.k8s.io/docs/user/configuration/#cluster-wide-options