# basens

## Description
kpt package for provisioning namespace

## Usage

### Fetch the package
`kpt pkg get REPO_URI[.git]/PKG_PATH[@VERSION] basens`
Details: https://kpt.dev/reference/cli/pkg/get/

### View package content
`kpt pkg tree basens`
Details: https://kpt.dev/reference/cli/pkg/tree/

### Apply the package
```
kpt live init basens
kpt live apply basens --reconcile-timeout=2m --output=table
```
Details: https://kpt.dev/reference/cli/live/

## Development
- Set a namespace:
```shell
kpt fn eval --type mutator --keywords namespace --image set-namespace:v0.4.1 --fn-config package-context.yaml
```

- Add setter mutator to the kptfile
```shell
kpt fn eval -i set-namespace:v0.4.1 --fn-config package-context.yaml --save -t mutator
```
