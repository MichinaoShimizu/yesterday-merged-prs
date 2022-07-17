# Yesterday Mereged PRs

Github Actions that reports all Pull Requests merged yesterday with indicators.

## Usage

```yaml
uses: MichinaoShimizu/yesterday-merged-prs@v2
```

## Example

```yaml
name: Yesterday Mereged PRs

on:
  workflow_dispatch: {}

jobs:
  reporting:
    runs-on: ubuntu-latest
    timeout-minutes: 3
    steps:
      - uses: actions/checkout@v3
      - uses: MichinaoShimizu/yesterday-merged-prs@v2
```
