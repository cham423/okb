# Live Host Data

### Buy Pick: Shodan

[https://www.shodan.io](https://www.shodan.io)

#### Details

* $69 - $1099 per month depending on number of results per month needed
* 1 million, 20 million, or unlimited results options
* 137,390,036 results for port:443

#### Usage Tips

* use `net:127.0.0.1/8` for searching for results in a CIDR network
* supports JARM searches with `ssl.jarm` parameter
* can stack queries i.e. `ssl.jarm:"2ad2ad16d2ad2ad22c42d42d000000dc2b105e4dda975fa70719c0cae5d0ce" net:203.97.69.74/24`
* supports organization filters i.e. `org:"Verizon Business"`
* supports SSN cert CN filters i.e. `ssl.cert.subject.cn:"*.google.com"`

### BinaryEdge

[https://www.binaryedge.io/](https://www.binaryedge.io/)

* free account available, 250 requests per month
* also gathers torrent/DHT data
* $10-500 a month for higher query limits
* 163,691,756 results for port:443

### LeakIX

[https://leakix.net/](https://leakix.net/)

* gray hat scanning platform
* targeted at identifying vulnerable services, but can be used for other things
* has "reporting" capability where vulnerabilities can be reported to their owners

### RiskIQ Community

[https://community.riskiq.com](https://community.riskiq.com)

* free account with business email has the following monthly quotas:

```
Web Searches: 350
API Searches: 3,500
Community (public) Projects: 1,000
Team & Analyst (private) Projects: 1
Basic Monitors: 5,000
Keyword Monitors: 10
Monitor Frequency: Weekly
Quota Duration
Monthly
Last Reset
2022-10-01 00:00:00
Next Reset
2022-11-01 00:00:00
```

* recently acquired by microsoft, integrated into Defender Threat Intelligence so future uncertain

### Greynoise

[https://viz.greynoise.io/](https://viz.greynoise.io/)

* "GreyNoise is a cybersecurity platform that collects and analyzes Internet-wide scan and attack traffic"
* does not scan the internet, but collects data on what is scanning/attacking from the internet

### Censys

[https://search.censys.io/](https://search.censys.io/)

* 96,166,688 results for port:443

### Netlas

[https://netlas.io](https://netlas.io)

### Onyphe

[https://www.onyphe.io/pricing/](https://www.onyphe.io/pricing/)

* 59 Euros for search access
* 100-1000 Euro plans for business
* unknown data size

### Build Pick: N/A

* most users should not try to scan the whole internet
* if you are the person that needs to build this, hopefully you know what you're doing&#x20;
