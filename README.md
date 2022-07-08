# Yesterday Mereged PRs

Github Actions that reports all Pull Requests merged yesterday with indicators.

## Usage

```yaml
name: Yesterday Mereged PRs

on:
  schedule:
    - cron: '0 2 * * 2-6'

  workflow_dispatch:

jobs:
  reporting:
    runs-on: ubuntu-latest
    timeout-minutes: 3
    steps:
      - uses: actions/checkout@v3
      - uses: MichinaoShimizu/yesterday-merged-prs@main
```

## Input

N/A

## Output

N/A
