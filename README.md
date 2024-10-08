[//]: # (mint token spl package ts)
[//]: # (https://github.com/Merstab/zeta-py-client)

# pyzeta

Python SDK to interact with Zeta

## Local Development / Testing

- Create a virtual environment

```bash
python3 -m venv myenv
```

- Activate the virtual environment

```bash
source myenv/bin/activate
```
- Run `pip install -r requirements-dev.txt` to do an editable install
- Run `pytest` to run tests

## Type Checking

Run `mypy .`

## Create and upload a package to PyPI

Make sure to bump the version in `setup.cfg`.

Then run the following commands:

```bash
rm -rf build dist
python setup.py sdist bdist_wheel
```

Then upload it to PyPI using [twine](https://twine.readthedocs.io/en/latest/#installation):

```bash
twine upload dist/*
```
