# minikube

```bash
docker image save gcr.io/k8s-minikube/kicbase:v0.0.27 -o kicbase:v0.0.27.tar

brew install git-lfs
git lfs install

git lfs track "*.psd"
git add . && git commit -m "Re-Add minikube image" && git push

docker image load -i kicbase:v0.0.27.tar
docker tag kicbase:v0.0.27 gcr.io/k8s-minikube/kicbase:v0.0.27
```
