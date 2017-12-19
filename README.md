# DucatusCoin

## Overview

DucatusCoin is a scrypt-based cryptocurrency.

DucatusCoin Core integration/staging tree
=====================================

What is DucatusCoin?
----------------

DucatusCoin is a digital currency that enables instant payments to anyone,
anywhere in the world. DucatusCoin uses peer-to-peer technology to operate with
no central authority: managing transactions and issuing money are carried out
collectively by the network. DucatusCoin Core is the name of open source
software which enables the use of this currency.

For more information, see [https://network.ducatus.net/](https://network.ducatus.net/).

License
-------

DucatusCoin Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/Ducatus/ducatuscoin-core/tags) are created
regularly to indicate new official, stable release versions of DucatusCoin Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).

Testing
-------

This is a security-critical project where any mistake may be costly. As such,
we have a rigorous project to test pull requests and may be slow to incorporate
requests and changes.

### Automated Testing

Developers are strongly encouraged to write [unit tests](/doc/unit-tests.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`

There are also [regression and integration tests](/qa) of the RPC interface, written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/qa) are installed) with: `qa/pull-tester/rpc-tests.py`

The Travis CI system makes sure that every pull request is built for Windows, Linux, and OS X, and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

ALl changes will be tested by Ducatus staff prior to being incorporated into
`master`. It is useful to add a test plan to the pull request description if
testing the changes will not be straightforward.

Translations
------------

We only accept translation fixes that are submitted through [Bitcoin Core's Transifex page](https://www.transifex.com/projects/p/bitcoin/).
Translations are migrated to DucatusCoin periodically.

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.
