# Yesterday Mereged PRs

Github Actions that reports all Pull Requests merged yesterday with indicators.

## Usage

```yaml
name: Daily Reporting

on:
  schedule:
    - cron: '0 2 * * 2-6'

  workflow_dispatch:

jobs:
  report-yesterday-merged-prs:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: MichinaoShimizu/yesterday-merged-prs@main
```

## Input

N/A

## Output

N/A
