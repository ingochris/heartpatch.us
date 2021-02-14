![Logo](https://i.imgur.com/hISnxYT.png)

# heartpatch.us (Under Construction) ![beating](https://i.imgur.com/IvHpVJJ.gif)
_Patching heartbleed openssl vulnerabilities on servers across the world wide web._

## Inspiration
>Heartbleed is a security bug in the OpenSSL cryptography library, which is a widely used implementation of the Transport Layer Security (TLS) protocol. It was introduced into the software in 2012 and publicly disclosed in April 2014. Heartbleed may be exploited regardless of whether the vulnerable OpenSSL instance is running as a TLS server or client. It results from improper input validation (due to a missing bounds check) in the implementation of the TLS heartbeat extension. Thus, the bug's name derives from heartbeat. The vulnerability is classified as a buffer over-read, a situation where more data can be read than should be allowed.

>The Electronic Frontier Foundation, Ars Technica, and Bruce Schneier all deemed the Heartbleed bug "catastrophic". Forbes cybersecurity columnist Joseph Steinberg wrote:
Some might argue that Heartbleed is the worst vulnerability found (at least in terms of its potential impact) since commercial traffic began to flow on the Internet.

>On the day of disclosure, The Tor Project advised:
If you need strong anonymity or privacy on the Internet, you might want to stay away from the Internet entirely for the next few days while things settle.

For such a critical bug that was unvealed years ago in 2014, there are still far too many unpatched systems on the internet, not to mention systems off the internet. A Shodan (search engine of internet-connected things via service banners) search for vuln:cve-2014-0160 from 2019 revealed 91,063 devices on the internet were still running OpenSSL versions still vulnerable to this critical exploit. [Archived Report](https://web.archive.org/web/20190711082042/https://www.shodan.io/report/0Wew7Zq7)

|Nation|Vulnerable Servers Online  |
|-|-|
|United States | 21,258 |
|China|8,655|
|Germany|5,647|
|Russian Federation|3,869|
|France|3,660|
|Korea, Republic of|3,407|
|Italy|2,858|
|Taiwan|2,639|
|Japan|2,368|
|United Kingdom|2,176|


## What it does
Heartpatch.us is a toolkit that includes modules to both scan and patch Heartbleed vulnerabilities.

## How it was built
From the main site, users are able to scan target servers to scan for Heartbleed vulnerability.

For servers not on the internet, users may use ssltest.sh to scan. From the report, unpatched servers are then prompted to run the patch script.

## Testing Instructions
Use the included Ubuntu 13.04 server virtual machine or docker containers to simulate Heartbleed vulnerable servers.

Nmap script can be used to scan for Heartbleed.

Metasploit MSFConsole has modules for exploitation.

## Attributes
Metasploit Heartbleed Exploit Auxillary Module

Nmap Project 

Nmap ssl-heartbleed script: https://nmap.org/nsedoc/scripts/ssl-heartbleed.html

FiloSottile's Heartbleed Scanner written in the Go language: https://github.com/FiloSottile/Heartbleed

Official Red Hat offline scanner written in the Python language by Katie Stafford: https://web.archive.org/web/20140412152427/https://access.redhat.com/labs/heartbleed/heartbleed-poc.py

The logo of the heartbleed bug (CC0 license): https://en.wikipedia.org/wiki/Heartbleed#/media/File:Heartbleed.svg

The Bandaid Cross Asset: https://wikiclipart.com/bandaid-clipart_24416/
