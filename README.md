# phone-channel

[![](https://images.microbadger.com/badges/image/newtonsystems/tools-phone-channel:0.2.2.svg)](https://microbadger.com/images/newtonsystems/tools-phone-channel:0.2.2 "Get your own image badge on microbadger.com")

[![](https://images.microbadger.com/badges/version/newtonsystems/tools-phone-channel:0.2.2.svg)](https://microbadger.com/images/newtonsystems/tools-phone-channel:0.2.2 "Get your own version badge on microbadger.com")

Available from docker hub as [newtonsystems/tools/phone-channel](https://hub.docker.com/r/newtonsystems/tools-phone-channel/)

#### Supported tags and respective `Dockerfile` links

-    [`v0.2.2`, `v0.2.1`, `v0.2.0`, `latest` (/Dockerfile*)](https://github.com/newtonsystems/devops/blob/master/tools/phone-channel/Dockerfile)

# What is phone-channel?

A base docker image to be used for circleci for compiling and building grpc services.


## How to use with circleci

- Example curl command

```bash
curl -H "Content-Type: application/json" -X POST -d '{"Name":"abc"}' http://`minikube ip`:32000/sayhello
```


curl -H "Content-Type: application/json" -X POST -d '{"Name":"abc"}' http://`minikube ip`:32000/sayhello 






## How to do a release
- Make sure you are using docker-utils 
i.e.

```bash
export PATH="~/<LOCATION>/docker-utils/bin:$PATH"
```

```
build-tag-push-dockerfile.py  --image "newtonsystems/tools-phone-channel" --version 0.1.0 --dockerhub_release --github_release
```


## Future

- Use docker when in development 
