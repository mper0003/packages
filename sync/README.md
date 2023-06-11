# sync

## Description
kpt package for provisiong application sync

## Usage

### Fetch the package
`kpt pkg get REPO_URI[.git]/PKG_PATH[@VERSION] sync`
Details: https://kpt.dev/reference/cli/pkg/get/

### View package content
`kpt pkg tree sync`
Details: https://kpt.dev/reference/cli/pkg/tree/

### Apply the package
```
kpt live init sync
kpt live apply sync --reconcile-timeout=2m --output=table
```
Details: https://kpt.dev/reference/cli/live/
