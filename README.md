# renovate-dry-run-action
Dry-run Renovate and print logs for GitHub Actions.

![](preview.png)

## Usage

See [action.yaml](action.yaml)

```yaml
jobs:
  renovate-dry-run:
    permissions:
      contents: read  # required by actions/checkout
      pull-requests: read  # required by renovate, because renovate to read pull request.
      issues: read  # required by renovate, because renovate to read issues.
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: cybozu/renovate-dry-run-action@v2
        with:
          config-file: renovate.json
```


## Release
1. Open [Tagging and Release action page](https://github.com/korosuke613/renovate-dry-run-action/actions/workflows/release.yaml).
2. Click `Run workflow`.
3. Input version.
4. Click `Run workflow`.
5. Open Releases page.
6. Amend draft release.
7. Uncheck `Set as a pre-release`.
8. Click `Update release`.
