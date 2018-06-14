# Spyder Plugin Cookiecutter

[![license](https://img.shields.io/pypi/l/spyder-plugin-cookiecutter.svg)](./LICENSE.txt)
[![pypi version](https://img.shields.io/pypi/v/spyder-plugin-cookiecutter.svg)](https://pypi.org/project/spyder-plugin-cookiecutter/)
[![conda version](https://img.shields.io/conda/v/spyder-ide/spyder-plugin-cookiecutter.svg)](https://www.anaconda.com/download/)
[![download count](https://img.shields.io/conda/d/spyder-ide/spyder-plugin-cookiecutter.svg)](https://www.anaconda.com/download/)
[![OpenCollective Backers](
https://opencollective.com/spyder/backers/badge.svg?color=blue)](#backers)
[![Join the chat at https://gitter.im/spyder-ide/public](https://badges.gitter.im/spyder-ide/spyder.svg)](
https://gitter.im/spyder-ide/public)

[![PyPI status](https://img.shields.io/pypi/status/spyder-plugin-cookiecutter.svg)](https://github.com/spyder-ide/spyder-plugin-cookiecutter)
[![CircleCI](https://circleci.com/gh/spyder-ide/spyder-plugin-cookiecutter/tree/master.svg?style=shield)](https://circleci.com/gh/spyder-ide/spyder-plugin-cookiecutter/tree/master)

----

## Plugin development paused until Spyder 4 release

Currently, work on official Spyder plugins is paused to focus our limited
resources on the development and release of Spyder 4, the next generation
of the Scientific Python Development Environment. Thanks to your continuing
support, we are on track for the final release of Spyder 4 in early 2019
with many highly anticipated features, including exposing a new public API for
external plugins, to make them easier to develop and more powerful.
Once that happens, active plugin development will resume, to add new features
and fix outstanding bugs. However, organizations or the community are welcome
to offer funding to continue development sooner; if so, please [contact us](
mailto:ccordoba12@gmail.com)!

Spyder development is made possible by contributions from our global user
community, along with organizations like [NumFOCUS](
https://www.numfocus.org) and [Quansight](https://www.quansight.com).
There are numerous [ways you can help](
https://github.com/spyder-ide/spyder/wiki/Contributing-to-Spyder),
many of which don't require any programming. If you'd like to [donate](
https://opencollective.com/spyder/donate) to help fund further improvements,
check us out on [OpenCollective](https://opencollective.com/spyder).

Thanks for all you do to make the Spyder project thrive! [More details](
https://github.com/spyder-ide/spyder/wiki/Current-Funding-and-Development-Status)

----

## Overview

Powered by [Cookiecutter](https://github.com/audreyr/cookiecutter) :cookie:, Spyder Plugin Cookiecutter is a template for jumpstarting [Spyder IDE](https://github.com/spyder-ide/spyder) :spider_web: plugins quickly.

> We recommend using conda and anaconda when developing a Spyder-IDE plugin.

## Features

- Compatible with Spyder >=3.1 and Spyder 4
- Follows Spyder Plugin Structure (`plugin.py`, `widgets`, `assets`, `tests`)
- A functional basic plugin.

### Repo structure
- `License.txt`, `MANIFIEST.in`, `CONTRIBUTORS.md` and `.gitatributes`
- `README.rst` with bagdes and some instructions.

### Packaging

- `requirements.txt` file for easy install dependencies for development
- `setup.py`
- Recipe files for creating conda package.

### Testing and Continuous Integration

- pytest configuration, and a basic test
- Integration with [Appveyor](https://www.appveyor.com/) for windows testing.
- Integration with [Circle-CI](https://circleci.com/) for linux testing.

### Code Checking

- Test Coverage with [Coveralls](https://coveralls.io/) Integration.
- Integration with [ciocheck](https://github.com/ContinuumIO/ciocheck/) for linting and codestyle checking
- Integration with [Scrutinizer CI](https://scrutinizer-ci.com/) for Code Quality

### Repo Managing

- (Optional) Version managing with  [versioneer](https://github.com/warner/python-versioneer)


## Usage

First, get Cookiecutter:

```
$ conda install "cookiecutter>=1.4.0"
```

If you want to use versioneer: (also you need to install git)

```
$ conda install versioneer
```

Now run against the repo:

```
$ cookiecutter gh:spyder-ide/spyder-plugin-cookiecutter
```

You'll be prompted for some values. and after that the repo will be generated

Normally you don't need to change `project_name` and `repo_name`.

Example:

```
author [Spyder Project Contributors]:
email [admin@spyder-ide.org]:
github_username [spyder-ide]:
plugin_name [Demo Plugin]: Reports
repo_name [spyder-reports]:
project_name [spyder_reports]:
description [Plugin for Spyder IDE.]: Spyder Plugin for Markdown reports for Pweave
version [0.1.0]:
create_config_page [n]:
use_ciocheck [y]:
support_python_2 [n]:
spyder3_compatibility [y]:
use_versioneer [y]:
```

## Testing

For testing you need to install pytest and pytest-cookies

```
$ pip install pytest pytest-cookies
```

And run pytest:

```
$ pytest
```

## Contributing

Everyone is welcome to contribute!

## Backers

Support us with a monthly donation and help us continue our activities.

[![Backers](https://opencollective.com/spyder/backers.svg)](https://opencollective.com/spyder#support)

## Sponsors

Become a sponsor to get your logo on our README on Github.

[![Sponsors](https://opencollective.com/spyder/sponsors.svg)](https://opencollective.com/spyder#support)
