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

Note this requires `conda install anaconda-client`

Conda environments can also be uploaded:

```shell
anaconda upload -d <description> environments/<name>.yaml
```

This can be created locally using:

```shell
conda env create cjs14/<name>
conda activate <name>
```
