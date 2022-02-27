

```
helm package myapp
mv myapp-0.2.0.tgz docs
helm repo index docs --url https://muhammedsaidkaya.github.io/chart-museum-test

helm repo add test https://muhammedsaidkaya.github.io/chart-museum-test
helm repo update
helm upgrade --install test test/myapp
```
