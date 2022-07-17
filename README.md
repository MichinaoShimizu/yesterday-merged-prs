# Yesterday Mereged PRs

Github Actions that reports all Pull Requests merged yesterday with indicators.

## Usage

## Example

```yaml
name: Yesterday Mereged PRs

on:
  schedule:
    - cron: '0 1 * * 2-5'

  workflow_dispatch:

jobs:
  reporting:
    runs-on: ubuntu-latest
    timeout-minutes: 3
    steps:
      - uses: actions/checkout@v3
      - uses: MichinaoShimizu/yesterday-merged-prs@v1
```
