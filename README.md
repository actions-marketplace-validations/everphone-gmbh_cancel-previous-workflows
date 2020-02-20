# cancel-previous-workflows
A Github action that cancels all previous workflows for older commits in its branch

## usage
```
name: Cancel

on: push

jobs:
  cancel:
    name: Cancel Previous Runs
    runs-on: ubuntu-latest
    steps:
      - name: cancel running workflows
        uses: everphone-gmbh/cancel-previous-workflows@v2
        env:
          GITHUB_TOKEN: ${{ github.token }}
```
