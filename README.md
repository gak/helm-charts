# Charts

## Overview

Use my repo:
```
helm repo add gak https://gak.github.io/helm-charts/
```

Use a chart, e.g. `pgdump-to-s3`:
```
helm install gak/pgdump-to-s3
```

## Notes

These are notes for myself before I automate:

### Package

```
helm package pgdump-to-s3
mv *tgz docs/
helm repo index docs/ --url https://gak.github.io/helm-charts/
# commit, push
```
