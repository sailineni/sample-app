## To build docker image & push it to Docker Hub Registry

```
docker login --> enter the user name & password of your account
docker build -t sailineni/sample-app:2.0 .
docker push sailineni/sample-app:2.0
```
## To deploy Docker image
```
k apply -f deploy-app.yml
```
## To expose the deployment, run the below command

```
k expose deployment sample-app --type=NodePort
```
