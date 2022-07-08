# Yesterday Mereged PRs

Github Actions that reports all Pull Requests merged yesterday with indicators.

## Usage

```yaml
name: Daily Reporting

on:
  schedule:
    cron: '0 2 * * 2-6'

  workflow_dispatch:

jobs:
  yesterday-merged:
    runs-on: ubuntu-latest
    timeout-minutes: 5
    steps:
      - name: Create Yesterday Merged PRs ISSUE
        uses: MichinaoShimizu/yesterday-merged-prs
        with:
          label: hogehoge
```

## Input

| key   | description             | required | default |
| ----- | ----------------------- | -------- | ------- |
| label | Label attached to ISSUE | false    | report  |

## Output

TBD
