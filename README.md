# g8stor-client-pypi
This is the pypi repository used to upload the g8storclient.

The binary module itself can be found here: https://github.com/nimscale/stor/

The current implementation used can be found here: https://github.com/maxux/libg8stor/

# Content of the package
This package contains binaries produced from the nim-lang version of our g8stor-client.

This repositories contains some architectures supported and the best one is selected during package setup.

# Installation
Contents provide the ability to install this package via pip.
```
pip3 install g8storclient
```

# Usage
When the package is installed, you can import `g8storclient`.

This is a minimal example, more can be found on the [nimscale/stor](https://github.com/nimscale/stor) repository.

```python
from g8storclient import g8storclient
client = g8storclient.connect("172.17.0.1")

uploaded = g8storclient.upload(client, "/tmp/file")
g8storclient.download(client, "/tmp/download", uploaded)
```
