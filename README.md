# dnslocal-windows-server
Build public DNS server on Windows Server to avoid DNS poisoning.


![](http://i.imgur.com/B9Bsvsy.png)

## Features

* Secure https update access.
* Automatically DNS rule update.
* Service auto start on reboot.
* Both IPv4 and IPv6 are supported.
* New version auto discovery.

## Supported domain

If you want to know all supported domains, Please refer to https://github.com/dnslocal/dnslocal-list

## Demo

* DNS: 123.206.16.184
* Replace http with https before access blocked sites 
* For HSTS support, please refer to implementation of dnslocal, such as [dnslocal-windows](https://github.com/dnslocal/dnslocal-windows)

```console
$ nslookup google.com 123.206.16.184
Server:		123.206.16.184
Address:	123.206.16.184#53

Non-authoritative answer:
Name:	google.com
Address: 220.255.2.153
```

## Download

You can always get the latest release here: https://github.com/dnslocal/dnslocal-windows-server/blob/master/RELEASE.md

## Requirement

* Windows Server 2008 or later required
* .NET Framework 4.5+ (not compatible with old version of Windows)

## Usage

Run DNSlocal.exe as administrator, please click update button to update configuration first, and click start button to run DNSlocal service. After do this, the service run as a public dns server listening on 0.0.0.0:53.

## Thanks

This software is proudly using the open source classifieds software [DNSAgent](https://github.com/stackia/DNSAgent).

# License

The project is released under [MIT License](https://github.com/dnslocal/dnslocal-list/blob/master/LICENSE).
