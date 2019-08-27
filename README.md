# Simple NPM Test

This action executes a `npm test` command on your repository. You can customize the command used by speicifying it as the `command` input in your workflow.

## Example

```yaml
jobs:
  test:
    name: 'Npm test'
    steps:
      - uses: @jsmrcaga/action-npm-test@v1
        with:
          command: 'my custom npm test --command'

```

## Disclaimer
This action is obviously not suited for production use, as it was a test I made. In order to run your own npm test please use:


```yaml
jobs:
  test:
    name: 'Npm test'
    steps:
      - run: 'npm test'

```
