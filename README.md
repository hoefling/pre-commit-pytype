# pre-commit for pytype
Wrapper to enable pre-commit for `pytype`

## Usage:
In your `.pre-commit-config.yaml` include the following block.

```
-   repo: https://github.com/hoefling/pre-commit-pytype
    rev: 2022.11.29
    hooks:
    -   id: pytype
```

If you use `setup.cfg` instead of `--config=pytype.cfg` to run pytype then you will also need to include a empty args attribute in the pytype hook (example below).

```
-   repo: https://github.com/hoefling/pre-commit-pytype
    rev: 2022.11.29
    hooks:
    -   id: pytype
        args: []
```
