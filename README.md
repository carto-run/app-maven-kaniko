# app-maven-kaniko

## Creating the Workload

```
tanzu apps workload create app-maven-kaniko \
  --namespace dev \
  --git-branch main \
  --git-repo https://github.com/carto-run/app-maven-kaniko \
  --label apps.tanzu.vmware.com/has-tests=true \
  --label app.kubernetes.io/part-of=app-maven-kaniko \
  --type web \
  --param dockerfile=./Dockerfile \
  --yes
```
