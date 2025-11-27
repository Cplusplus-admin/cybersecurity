# 🟢 Connection Tester

<figure><img src="../../../../.gitbook/assets/image (66).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../.gitbook/assets/image (67).png" alt=""><figcaption></figcaption></figure>

normal login page and don't worry about 304 status we can just remove If-None-Match request header and it will show login page or just clear browser cache

so back to the topic we will test login page with sqli payload, deleting parameter, blank password etc

<figure><img src="../../../../.gitbook/assets/image (68).png" alt=""><figcaption></figcaption></figure>

ok it worked with sqli payload

```
admin'--
```

<figure><img src="../../../../.gitbook/assets/image (69).png" alt=""><figcaption></figcaption></figure>

interesting seen this before also i think in htb where it leads to RCE

<figure><img src="../../../../.gitbook/assets/image (70).png" alt=""><figcaption></figcaption></figure>

may be let's try using bash command separator

<figure><img src="../../../../.gitbook/assets/image (71).png" alt=""><figcaption></figcaption></figure>

different result

<figure><img src="../../../../.gitbook/assets/image (72).png" alt=""><figcaption></figcaption></figure>

Got it

```
;ls;
```

<figure><img src="../../../../.gitbook/assets/image (73).png" alt=""><figcaption></figcaption></figure>
