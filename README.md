# helm-chart - update (in linux prompt)

```
# helm package deploy/kcm-agent/
# --> kcm-agent-0.0.1.tgz 
# helm repo index --url https://yoonseongduk.github.io/helm-charts/ . 
# --> index.yaml 
#
```

# git push (update)

```
# git status
# git add .
# git commit -m 'helm-charts update'
# git push origin main
```

# helm-charts - install

```
# kcm-workdir="/root/kcmagent"
# cd ${kcm-workdir}
# cd ./deploy/kcm-agent
# helm repo add kcmagent https://yoonseongduk.github.io/helm-charts
# helm repo update
# helm repo list
# helm dependency update
# helm template -f ../../values.yaml .   