---
description: 'inputs: username | outputs: list of profiles associated with that username'
---

# Profile Discovery by Username

## Testing Methodology

1. check the same username (i.e. cham423) using each tool
   * count the number of profiles discovered
   * count number of false positives (nonexistent profiles, not mismatches)
2. rate difficulty of deployment
3. rate quality of output
4. rate development health
5. rate automation potential

{% hint style="info" %}
see the template at the bottom of the page if you are adding a new tool.
{% endhint %}

## CLI Pick

### Sherlock

{% embed url="https://github.com/sherlock-project/sherlock" %}

#### Example Results

```shell
python3 sherlock.py cham423 -o cham423.out
```

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

* 38 total results
* 0 false positives!
* 7 results were not the target, but were valid accounts

#### Deployment

* python (medium difficulty)
* has a docker container as a fallback

#### Output

* basically stdout, no JSON output option -- a list of discovered profile urls

#### Development Health

* very healthy, recent commits, large number of contributors, long history

#### Automation Potential

* very high, command line tool that supports input lists
* \<todo> not tested at scale. from a single host, would likely encounter rate limiting when enumerating large numbers of profiles

## Web Pick: whatsmyname.app

[https://whatsmyname.app](https://whatsmyname.app)

#### Example Results

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

* 34 total results
* 0 false positives!

#### Deployment

* easy, web hosted

#### Output <a href="#output" id="output"></a>

* Clickable links, clipboard copy, excel, CSV, PDF

#### Development Health <a href="#development-health" id="development-health"></a>

* Well supported/maintained.

#### Automation Potential <a href="#automation-potential" id="automation-potential"></a>

* No captcha. there is an accompanying CLI tool, but it doesn't seem to function as well, with more false positive

## Other Tools

### WhatsMyName

{% embed url="https://github.com/WebBreacher/WhatsMyName" %}

#### Example Results

```shell
 python3 whats_my_name.py -u cham423 -o cham423.out
```

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

* 114 total results
* 75 false positives! (65% false positive rate)

{% hint style="danger" %}
_Note: I am not sure why the CLI version of this tool has so many false positives. The web-hosted version (whatsmyname.app) is excellent._&#x20;
{% endhint %}

#### Deployment

* python (medium difficulty)

#### Output

* file output was broken at time of testing (2022-09-18)
* stdout is printed in table form with lots of extra spaces/characters, and some profile links are cut off

#### Development Health

* good

#### Automation Potential

* medium -- this project is used by many projects for its JSON list of profile urls, which can be imported to check usernames automatically. the false positive rate is alarming

### Namechk (web)

{% embed url="https://namechk.com" %}

#### Example Results

<figure><img src="../../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

* 25 total results
* 1 false positive

#### Deployment

* web hosted (easy difficulty)
* 1-5 clicks to full results

#### Output

* No file output
* Profile links to signup/about pages, not valid profiles

#### Development Health

* unknown (third party)

#### Automation Potential

* very limited: captcha + cloudflare would prevent easy scraping

### namecheckr

{% embed url="https://www.namecheckr.com/" %}

#### Example Results

<figure><img src="../../.gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>

* 12 total results
* 1 false positives

#### Output <a href="#output" id="output"></a>

* no file output
* site links point to root page, not profile link

#### Development Health <a href="#development-health" id="development-health"></a>

* unknown (third party)

#### Automation Potential <a href="#automation-potential" id="automation-potential"></a>

* no CAPTCHA, so could be scraped



### UserSearch.org

{% embed url="https://usersearch.org/" %}

#### Example Results

<figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

* 15 total results
* 1 false positive

#### Deployment

* web hosted (easy difficulty)
* requires 10+ clicks to see all sites, no single page with all results

#### Output <a href="#output" id="output"></a>

* no file output
* profile links available in search results, but not on single page

#### Development Health <a href="#development-health" id="development-health"></a>

* unknown (third party)

#### Automation Potential <a href="#automation-potential" id="automation-potential"></a>

* no CAPTCHA, could potentially be scraped

### NameCheckup

{% embed url="https://namecheckup.com/" %}

#### Example Results

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

* 14 total results
* 1 false positive

#### Deployment

* web hosted (easy difficulty)
* 1-5 clicks to results

#### Output <a href="#output" id="output"></a>

* no file output
* results link to specific profiles

#### Development Health <a href="#development-health" id="development-health"></a>

* unknown (third party)

#### Automation Potential <a href="#automation-potential" id="automation-potential"></a>

* no CAPTCHA, could potentially be scraped

### CheckUsernames

{% embed url="https://checkusernames.com/" %}

#### Example Results

<figure><img src="../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

* 42 total results
* 27 false positives
* 79 errors checking target site

#### Deployment

* web hosted (easy difficulty)
* 1-5 clicks to results

#### Output <a href="#output" id="output"></a>

* no file output
* profile links are to individual profile, not to root page which is nice

#### Development Health <a href="#development-health" id="development-health"></a>

* unknown (third party)

#### Automation Potential <a href="#automation-potential" id="automation-potential"></a>

* no CAPTCHA, could potentially be scraped

### Namechk (script)

{% hint style="danger" %}
This tool is not currently functional as of 2022-09-18, and returns all false positives due to Cloudflare bot protection
{% endhint %}

{% embed url="https://github.com/GONZOsint/Namechk" %}

#### Example Output

<figure><img src="../../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

### Todo

* [https://knowem.com/](https://knowem.com/)
* [https://instantusername.com/#/](https://instantusername.com/#/)
* namevine
* socialsearcher

### Template

\<link to tool>

#### Example Results

* n total results
* n false positives

#### Deployment

#### Output <a href="#output" id="output"></a>

* \<describe output options>

#### Development Health <a href="#development-health" id="development-health"></a>

* \<describe project health>

#### Automation Potential <a href="#automation-potential" id="automation-potential"></a>

* \<describe automation potential>

