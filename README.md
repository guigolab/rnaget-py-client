# rnaget client

 > An easy-to-use python client to query the GA4GH RNAget compliant server.

[![PyPI version][pypi-image]][pypi-url]
[![Build status][build-image]][build-url]
[![Code coverage][coverage-image]][coverage-url]
[![GitHub stars][stars-image]][stars-url]
[![Support Python versions][versions-image]][versions-url]


## Getting started

You can [get `rnaget-client` from PyPI](https://pypi.org/project/rnaget-client),

```bash
python -m pip install rnaget-client
```


## Example usage

The constructor accepts the following arguments:

    host : here you can specify the URL of the host server, other accepted values or 'gtex' or 'encode' to directly connect to the GTEX or ENCODE RNAget instances
    token : string
        The access token used to access protected data (if implemented by the host server)
    service_info: boolean
        When set to true it will print the service info of the host server when succesfully connecter

```py
from rnaget_client import RnaGet

gtex = RnaGet(host='gtex') # gtex instance
encode = RnaGet(host='encode') # encode instance
another_host = RnaGet(host='ANOTHER_URL', token='ACCESS_TOKEN')


```

Refer to [this article](https://mathspp.com/blog/custom-json-encoder-and-decoder) to learn more about the internal details of `extendedjson`.


## Changelog

Refer to the [CHANGELOG.md](CHANGELOG.md) file.


<!-- Badges -->

[pypi-image]: https://img.shields.io/pypi/v/extendedjson
[pypi-url]: https://pypi.org/project/extendedjson/
[build-image]: https://github.com/mathspp/extendedjson/actions/workflows/build.yaml/badge.svg
[build-url]: https://github.com/mathspp/extendedjson/actions/workflows/build.yaml
[coverage-image]: https://codecov.io/gh/mathspp/extendedjson/branch/main/graph/badge.svg
[coverage-url]: https://codecov.io/gh/mathspp/extendedjson/
[stars-image]: https://img.shields.io/github/stars/mathspp/extendedjson
[stars-url]: https://github.com/mathspp/extendedjson
[versions-image]: https://img.shields.io/pypi/pyversions/extendedjson
[versions-url]: https://pypi.org/project/extendedjson/
