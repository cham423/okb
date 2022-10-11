---
description: 'input: domains | output: list of emails for input domains'
---

# Email Enumeration by Domain

## Testing Methodology

1. check the same domain (i.e. microsoft.com) using each tool
   * count the number of results
2. rate difficulty of deployment
3. rate quality of output
4. rate development health
5. rate automation potential

### Hunter&#x20;

{% embed url="https://hunter.io/search" %}

#### Example Results

<figure><img src="../../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

* 35,830 results
* also shows email format (i.e. {f}.{last}@domain.com

#### Deployment Difficulty

* web hosted (easy difficulty)
* has API

#### Output

* can export subset of records from web interface
* can export full records using API (if credits available in account)

#### Pricing

* $50-400/month depending on plan
* free plan available, limited quota per month



### Infoga

\<todo>

{% embed url="https://github.com/m4ll0k/infoga" %}

* "Infoga is a tool gathering email accounts informations (ip,hostname,country,...) from different public source (search engines, pgp key servers and shodan) and check if emails was leaked using haveibeenpwned.com API"
* Language: python

### skymem.info

{% embed url="http://www.skymem.info/" %}

#### Example Results

<figure><img src="../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
**Note: i have not confirmed this is a legitimate site**
{% endhint %}

* 36631 results

#### Deployment Difficulty

* web hosted (easy difficulty)
* No API

#### Pricing

* varies by results size, not transparent
* large lists get into $2000-3000 range!!!
