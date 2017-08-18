HTTP Parser - Qompoter Wrapper
===========

This [Qompoter](https://github.com/Fylhan/qompoter) wrapper helps to integrate [nodejs/http-parser](https://github.com/nodejs/http-parser), a parser for HTTP messages written in C, using [Qompoter](https://github.com/Fylhan/qompoter).

Usage
-----------

To use [nodejs/http-parser](https://github.com/nodejs/http-parser) in a project, simply create (or update) the following `qompoter.json` file in your project root directoy:


```json
{
    "name": "acme/my-project",
    "require": {
        "qompoter/http-parser-wrapper": "v2.7.*"
    }
}
```

Then, download and install `http-parser` using Qompoter:

```bash
qompoter install
```

*Note: to install Qompoter on your machine, use `npm install -g qompoter` or check [Qompoter documentation](https://github.com/Fylhan/qompoter/blob/master/README.md#installation).*

That's it! Qompoter has downloaded `http-parser` into the `vendor` directory, you can now include `vendor.pri` in the `.pro` file of your project, and select `http-parser` as a dependency:

```qmake
CONFIG += http-parser
include(vendor/vendor.pri)
```

Let's start coding! Check [nodejs/http-parser examples](https://github.com/nodejs/http-parser#usage).
