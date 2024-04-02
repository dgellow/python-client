<!-- Begin Title, generated by Fern  -->
# Mixpeek Python Library

[![fern shield](https://img.shields.io/badge/%F0%9F%8C%BF-SDK%20generated%20by%20Fern-brightgreen)](https://github.com/fern-api/fern)

The Mixpeek Python Library provides convenient access to the Mixpeek API from applications written in Python.
<!-- End Title  -->

<!-- Begin Installation, generated by Fern  -->
# Installation

```sh
pip install --upgrade mixpeek
```
<!-- End Installation  -->

<!-- Begin Usage, generated by Fern  -->
# Usage

```python
from mixpeek.client import Mixpeek

client = Mixpeek(
    api_key="YOUR_API_KEY",
    base_url="https://yourhost.com/path/to/api",
)
```
<!-- End Usage  -->

<!-- Begin Async Usage, generated by Fern  -->
# Async Client

```python
from mixpeek.client import AsyncMixpeek

client = AsyncMixpeek(
    api_key="YOUR_API_KEY",
    base_url="https://yourhost.com/path/to/api",
)
```
<!-- End Async Usage  -->

<!-- Begin Status, generated by Fern  -->
# Beta Status

This SDK is in beta, and there may be breaking changes between versions without a major 
version update. Therefore, we recommend pinning the package version to a specific version. 
This way, you can install the same version each time without breaking changes.
<!-- End Status  -->

<!-- Begin Contributing, generated by Fern  -->
# Contributing

While we value open-source contributions to this SDK, this library is generated programmatically. 
Additions made directly to this library would have to be moved over to our generation code, 
otherwise they would be overwritten upon the next generated release. Feel free to open a PR as
 a proof of concept, but know that we will not be able to merge it as-is. We suggest opening 
an issue first to discuss with us!

On the other hand, contributions to the README are always very welcome!
<!-- End Contributing  -->

