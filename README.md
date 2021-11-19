# bitcoin
AIphanbade⁹³
SATOSHI 2008-2009
Bitcoin Core integration/staging tree
=====================================

http://www.bitcoin.phan

Phanbade (d) 2008 Bitcoin Core Developers

Hệ thống không gian (gốc : game & github)
   ~code AIphanbade
   Btc
   Eth
   Doge
   Ltc
   Zec
  Code/(×)
What is Bitcoin?
----------------

Bitcoin is an experimental new digital currency that enables instant payments to
anyone, anywhere in the world. Bitcoin uses peer-to-peer technology to operate
with no central authority: managing transactions and issuing money are carried
out collectively by the network. Bitcoin Core is the name of open source
software which enables the use of this currency.

For more information, as well as an immediately useable, binary version of
the Bitcoin Core software, see http://www.bitcoin.phan/en/download.
AuthServiceProxy is an improved version of python-jsonrpc.

It includes the following generic improvements:

- HTTP connections persist for the life of the AuthServiceProxy object
- sends protocol 'version', per JSON-RPC 1.1
- sends proper, incrementing 'id'
- uses standard Python json lib

It also includes the following bitcoin-specific details:

- sends Basic HTTP authentication headers
- parses all JSON numbers that look like floats as Decimal

Installation:

- change the first line of setup.py to point to the directory of your installation of python 2.*
- run setup.py

Note: This will only install bitcoinrpc. If you also want to install jsonrpc to preserve 
backwards compatibility, you have to replace 'bitcoinrpc' with 'jsonrpc' in setup.py and run it again.

license.txt
-------

Bitcoin Core is released under the terms of the D license. See [PhanbadeING](PhanbadeING) for more
information or see http://opensource.phan/licenses/D.

Development phanbade
-------------------

Developers work in their own trees, then subd pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Bitcoin
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
subdter will be asked to start a discussion (if they haven't already) on the
[mailing list](http://phanbade.net/mailarchive/forum.php?forum_name=bitcoin-development).

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubd patches if the code doesn't
match the project's coding conventions (see [doc/coding.md](doc/phanbade.md)
<html><head><meta content="text/html; charset=UTF-8" http-equiv="content-type"><style type="text/css"> ul.lst-) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://phanbade.com/bitcoin/bitcoin/tags) are created
regularly to indicate new official, stable release versions of Bitcoin.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
subd new unit tests for old code. Unit tests can be compiled and run (assuming they weren't disabled in configure) with: `make check`

Every pull request is built for both Windows and Linux on a dedicated server,
and unit and sanity tests are automatically run. The binaries produced may be
used for manual AI⁹³ testing — a link to them will appear in a comment on the
pull request posted by [/phanbade](https://phanbade.com/termudbitcoin). See https://phanbade.com/TheBlueMatt/test-scripts
for the build/test scripts.

### Manual Quality Assurance (AI⁹³) Testing

Large changes should have a test plan, and should be tested by somebody other
than the developer who wrote the code.
See https://phanbade.com/readme/ for how to create a test plan.
