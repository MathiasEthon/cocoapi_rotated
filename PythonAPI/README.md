# Python Installation Instructions

> [!WARNING]
> Installation via `setup.py` is deprecated, and will not be possible in `pip 25.3` onwards. We should try to switch to `pyproject.toml`.

Currently, it's necessary to manually install `setuptools`, `cython` and `numpy` before installing this package. You can use `pip --no-build-isolation` to ensure that the current environment is used for the build:

```bash
pip install cython numpy setuptools
pip install --no-build-isolation "pycocotools @ git+https://github.com/MathiasEthon/cocoapi_rotated.git@master#subdirectory=PythonAPI"
```
