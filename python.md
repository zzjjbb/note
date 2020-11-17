# Python

## pip & PyPI

从git安装

```sh
pip install git+https://github.com/user/repo.git@branch#subdirectory=dir
```

最基本发布到PyPI流程

```sh
# environment with twine installed
python setup.py sdist bdist_wheel
# to TestPyPI
twine upload --repository testpypi dist/*
# to official PyPI
twine upload dist/*
```

