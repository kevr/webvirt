webvirt
-------

A web-based frontend to libvirt.

The whole of webvirt depends on three seperate projects:

- libvirt API (C++) -- [webvirtd](https://github.com/kevr/webvirtd)
    - ![lint](https://github.com/kevr/webvirtd/actions/workflows/lint.yaml/badge.svg?branch=master) ![build](https://github.com/kevr/webvirtd/actions/workflows/build.yaml/badge.svg?branch=master) ![tests](https://github.com/kevr/webvirtd/actions/workflows/tests.yaml/badge.svg?branch=master) [![license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
    - UNIX socket authentication
- API (Django) -- [webvirt_api](https://github.com/kevr/webvirt_api)
    - ![lint](https://github.com/kevr/webvirt_api/actions/workflows/lint.yaml/badge.svg?branch=master) ![tests](https://github.com/kevr/webvirt_api/actions/workflows/tests.yaml/badge.svg?branch=master) [![license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
    - PAM authentication
    - JSON web token leasing
    - Proxies authenticated requests to [webvirtd](https://github.com/kevr/webvirtd)
- Front-end (React) -- [webvirt_react](https://github.com/kevr/webvirt_react)
    - ![lint](https://github.com/kevr/webvirt_react/actions/workflows/lint.yaml/badge.svg?branch=master) ![tests](https://github.com/kevr/webvirt_react/actions/workflows/react.yaml/badge.svg?branch=master) [![license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
    - Utilizes [webvirt_api](https://github.com/kevr/webvirt_api) as a back-end

All three aforementioned projects operate under the
[Apache 2.0 open license](https://www.apache.org/licenses/LICENSE-2.0).
