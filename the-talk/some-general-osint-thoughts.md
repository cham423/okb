# Some General OSINT Thoughts

### Consider OPSEC before you start

* your intelligence gathering is part of someone else's intelligence
* use a clean image if creating admissable evidence
  * Michael Bazzell has an excellent guide for this in his OSINT Techniques book

### Automate anything you can&#x20;

* build a simple API wrapper script
* consider storing it in jupyter
* at the very least, build a checklist/standard procedure to follow

### Always keep your output

* I prefer JSON/structured output formats, but you can parse it later
* Consider storing everything in elastic/ELK
  * Newer versions of ES are really good at auto-mapping
  * `curl -XPOST http://elk:9200/osint_dump_2022-09-15/_doc -H "Content-Type: application/json" -d @amass_out.json`
