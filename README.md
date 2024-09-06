## Getting started with basic drupal app

This is a simple example based on:

* **building** a `Dockerfile` using local docker to build
* **tagging** using the default tagPolicy (`gitCommit`)
* **deploying** a single container pod using `kubectl`

### Usage

```bash
skaffold config set --global local-cluster true
eval $(minikube docker-env)
skaffold dev --port-forward
```