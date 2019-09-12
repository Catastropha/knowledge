# Upload Python package to PyPI

1.  `pip install setuptools wheel twine` - installs required libraries
2.  `python setup.py sdist bdist_wheel` - before upload you have to build it
3.  `python -m twine upload dist/*` - upload. You'll be asked for credentials


