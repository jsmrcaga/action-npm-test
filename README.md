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
