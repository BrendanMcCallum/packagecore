How to Install
==============

Requirements
------------

PackageCore is written in Python 3, and makes use of the modules `PyYAML` and
`setuptools`. It utilizes `Docker` to build packages for each
distribution. Some of the installation methods below will install dependencies
for you.

In general, you should install the following packages for you system:

* `python3`

* `python3-setuptools`

* `python3-pyyaml`

* `docker`

If you install `PyYAML` via pip, you will also need to install
`libyaml`, the C library upon which it depends.


Via PyPI 
--------

For each PackageCore release we upload a signed package to
[PyPI](https://pypi.python.org). Before installing it you should install
`Docker` and `libyaml` on your system. Then simply retrieve the latest version
via `pip`:

```
pip install packagecore
```


Via pre-built Package
---------------------

On the [GitHub releases](https://github.com/BytePackager/packagecore/releases)
page, we provide several Linux packages for PackageCore.
These packages are generated by the Travis-CI job when a new tag is pushed to
the repository. Subsequently these packages are not signed.



From Source
-----------

You can also clone the latest version from
[GitHub](https://github.com/bytepackager/packagecore) and install it via the
python's `setuptools`:

```
git clone https://github.com/bytepackager/packagecore
./setup.py sdist
pip install dist/packagecore-X.X.X.tar.gz
```

Where `X.X.X` is the current version.

