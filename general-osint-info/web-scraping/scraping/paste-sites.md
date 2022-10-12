---
description: Paste sites are internet dumpsters, but dumpster diving can be rewarding
---

# Paste Sites

## Tools

### Pastehunter

{% embed url="https://github.com/kevthehermit/PasteHunter" %}

## Site Info

### Pastebin ([https://pastebin.com](https://pastebin.com/))

* 8 byte alphanumeric ID
* Provides scraping API with feeds, but requires grandfathered pro account

```python
# example
https://pastebin.com/Vqai8sBA
```

### [rentry.co](http://rentry.co/)

* 5 byte alphanumeric ID
* no feed

```python
# example
https://rentry.co/uvq4v
```

### zerobin ([https://zerobin.net](https://zerobin.net/))

```python
# example
https://zerobin.net/?98703897a0cdceef#uTVX3KoxQbNrDJE+efmO9sexX3jT6Zt0ed4glZj295U=
```

### [justpaste.it](http://justpaste.it/)

* no recent feed
* no API

```markdown
# example paste
https://justpaste.it/3spa1
```

### [twitlonger.com](http://twitlonger.com/) / [tl.gd](http://tl.gd/)

* oauth from twitter only
* no recent feed
* api is for getting/updating posts only, auth required
* 9 char id (alphanumeric with symbols)

```markdown
# example link
https://www.twitlonger.com/show/n_1s1vre6
http://tl.gd/n_1s1vre6
```

### [jsfiddle.net](http://jsfiddle.net/)

* 8 char id (alphanumeric)

```markdown
#example
https://jsfiddle.net/k092mfae/
```

### [gist.github.com](https://gist.github.com/)

* requires username
* 32 char id (hex)

```markdown
https://gist.github.com/cham423/308cba152d57d10d91a1dbd614768024
```

### Textbin ([https://textbin.net/](https://textbin.net/))

* recent paste list, HTML only (would have to be scraped, extracted from homepage)
  * embedded in homepage, no API, no dedicated HTML page)

```python
# example
https://textbin.net/1q09pepj0k
```

### ideone ([ideone.com](http://ideone.com/))

* IDE (sandbox code exec)
* has recent feed HTML ([https://ideone.com/recent](https://ideone.com/recent))

```python
# example
https://ideone.com/Ok8iWL
```

### pastesite ([https://pastesite.org/lists](https://pastesite.org/lists))

* very low volume
* has recent feed HTML ([https://pastesite.org/lists](https://pastesite.org/lists))

```python
# example
https://pastesite.org/view/19d5c69e
```

### controlC ([https://controlc.com](https://controlc.com))

* popular
* no recent feed
* 8 byte hex ID

```python
# example
<https://controlc.com/ff1435ac>
```

### ghostbin

[https://ghostbin.co](https://ghostbin.co/)

* defunct

### sources

[https://mediasonar.com/2020/09/09/pastebins-darkwebmarketplaces-osint/](https://mediasonar.com/2020/09/09/pastebins-darkwebmarketplaces-osint/)
