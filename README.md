# heartpatch.us

Heartbleed scan and patch tools

>Heartbleed is a security bug in the OpenSSL cryptography library, which is a widely used implementation of the Transport Layer Security (TLS) protocol. It was introduced into the software in 2012 and publicly disclosed in April 2014. Heartbleed may be exploited regardless of whether the vulnerable OpenSSL instance is running as a TLS server or client. It results from improper input validation (due to a missing bounds check) in the implementation of the TLS heartbeat extension. Thus, the bug's name derives from heartbeat. The vulnerability is classified as a buffer over-read, a situation where more data can be read than should be allowed.

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
