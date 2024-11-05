# Desafio DevOps & Cloud

Aula 1 - Desafio Docker | Primeiros passos em DevOps e Docker <br>
- Otimizado a imagem docker, reduzindo o tamanho de 1GB para 70MB.
```bash
docker build -t conversao-distancia -f Dockerfile .

docker container run -d -p 8181:5000 conversao-distancia
```

#

Aula 2 - Desafio Kubernetes | Do zero ao deploy
```bash
k3d cluster create cluster-aula-2 --servers 3 --agents 3 -p "8181:30000@loadbalancer"

kubectl apply -f k8s/deployment.yaml

```
