# Third-party notices

Mose Firewall includes or uses the following components.

## Included in the program

**libcolumnlistview** (the column list of the main window), part of the
Haiku development kit, linked into `MoseFirewall`. Haiku is distributed
under the MIT licence:

```
Copyright (c) 2001-2026 Haiku, Inc. and contributors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

The kernel add-on is built with configuration headers of the Haiku
source tree (`build/config_headers`), under the same MIT licence.

## Provided by the system

Not included in the packages, installed with Haiku:

- **Haiku** libraries (libbe, libnetwork, libbnetapi, libroot) — MIT
  licence.
- **OpenSSL 3** `libcrypto` (Haiku package `openssl3`), used to verify
  activation keys (Ed25519) — Apache License 2.0.

## ARM64 package only

There is no OpenSSL package for ARM64 Haiku yet, so the ARM64 package
includes **OpenSSL 3.5.7** `libcrypto`, unmodified, linked into the
programs. OpenSSL is licensed under the Apache License 2.0, included in
the package as `OpenSSL-LICENSE.txt`
(<https://www.openssl.org/source/license.html>).
