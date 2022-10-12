# Live Host Data

### Shodan

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
