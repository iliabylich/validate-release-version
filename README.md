# `validate-release-version`

A GH Action to validate that a version:

- follows `MAJOR.MINOR.PATCH` format
- is new (i.e. there's no `v<version>` tag)

## Usage

```yaml
steps:
  - uses: actions/checkout@v4
  - uses: iliabylich/validate-release-version@v1
    with:
      version: ${{ inputs.version }}
```
