# Action: Install Action Validator

The way to install the action validator requires the hardcoding of the version of the tool.
This action only exists to contain that hard coding within a single action for ease of maintenance.

## Usage

To use this action, include it in your workflow file. Here is an example:

```yaml
name: Install Action Validator
on: [push, pull_request]

jobs:
  install-action-validator:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout repository
        uses: actions/checkout@v4
      - name: Install Action Validator
        uses: meza/install-action-validator@v1
```
