# conda_recipes

Conda recipes for the [cjs14 repository](https://anaconda.org/cjs14/).

Generally they are initially created by:

```shell
conda skeleton pypi --output-dir recipes/ --noarch-python <package_name>
```

Linted by:

```shell
conda-smithy recipe-lint recipes/<package_name>
```

Then uploaded by:

```shell
conda-build recipes/<package_name>
```
