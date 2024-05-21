docker build -t viktor891/app:1.0 -f app/Dockerfile app/
docker build -t viktor891/script:1.0 -f script/Dockerfile script/

docker push viktor891/app:1.0
docker push viktor891/script:1.0

kubectl apply -f app-deployment.yaml
kubectl apply -f script-deployment.yaml