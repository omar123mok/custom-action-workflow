# Build Status Badge: ![custom-workflow](https://github.com/omar123mok/custom-action-workflow/workflows/cutsom/badge.svg)

# Custom-Action-workflow

This workflow is a demo of cutsom Action and this uses an Action defined on https://github.com/omar123mok/custom-action/tree/main

## Events
Push event is used to trigger the workflow

## Code

```yaml
name: custom
on: push
jobs:
  main:
    runs-on: ubuntu-latest
    steps:
      - uses: omar123mok/custom-action@main
```

The first step uses an action named omar123mok/custom-action@main.
This is the action provided on - https://github.com/omar123mok/custom-action/tree/main that will call the Dockerfile which then calls the entrypoint.sh script.
```
uses: omar123mok/custom-action@main
```
