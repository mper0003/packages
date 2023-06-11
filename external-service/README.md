# external-service

## Description
kpt package for provisiong services external to the cluster

## Usage

### Fetch the package
`kpt pkg get REPO_URI[.git]/PKG_PATH[@VERSION] external-service`
Details: https://kpt.dev/reference/cli/pkg/get/

### View package content
`kpt pkg tree external-service`
Details: https://kpt.dev/reference/cli/pkg/tree/

### Apply the package
```
kpt live init external-service
kpt live apply external-service --reconcile-timeout=2m --output=table
```
Details: https://kpt.dev/reference/cli/live/
