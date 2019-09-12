# Upload Python package to PyPI

1.  First, install required libraries: `pip install setuptools wheel twine`
2.  Whenever you want to upload a new version you first have to build it: `python setup.py sdist bdist_wheel`
3.  Finally, upload: `python -m twine upload dist/*`


