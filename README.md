# renovate-dry-run-action
Dry run Renovate and print logs for GitHub Actions.

![](preview.png)

## Usage

See [action.yaml](action.yaml)

```yaml
steps:
  - uses: actions/checkout@v3
  - uses: korosuke613/renovate-dry-run-action@v1
    with:
      config-file: renovate.json
```
