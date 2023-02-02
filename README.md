webvirt
-------

A web-based frontend to libvirt.

The whole of webvirt depends on three seperate projects:

- libvirt API (C++) -- [webvirtd](https://github.com/kevr/webvirtd)
    - UNIX socket authentication
- API (Django) -- [webvirt_api](https://github.com/kevr/webvirt_api)
    - PAM authentication
    - JSON web token leasing
    - Proxies authenticated requests to [webvirtd](https://github.com/kevr/webvirtd)
- Front-end (React) -- [webvirt_react](https://github.com/kevr/webvirt_react?target=_blank)
    - Utilizes [webvirt_api](https://github.com/kevr/webvirt_api) as a back-end

All three aforementioned projects operate under the
[Apache 2.0 open license](https://www.apache.org/licenses/LICENSE-2.0).
