

~~~~
david@ThinkpadT420:~$ python3
Python 3.8.5 (default, Jul 28 2020, 12:59:40) 
[GCC 9.3.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import requests
>>> url = "https://192.168.1.254"
>>> r = requests.get(url, allow_redirects=True)
>>> print(r.contents)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
AttributeError: 'Response' object has no attribute 'contents'
>>> r
<Response [200]>
>>> print(r.content) 
b'<!doctype html>\n<head>\n  <meta http-equiv="X-UA-Compatible" content="IE=Edge;chrome=1" />\n  <meta charset="utf-8">\n  <meta name="viewport" content="width=device-width, initial-scale=1.0">\n 
~~~~


References:
https://deliciousbrains.com/ssl-certificate-authority-for-local-https-development/
https://www.stevejenkins.com/blog/2015/10/install-an-ssl-certificate-on-a-ubiquiti-edgemax-edgerouter/
https://serverfault.com/questions/485597/default-ca-cert-bundle-location
https://www.digitalocean.com/community/tutorials/how-to-set-up-and-configure-a-certificate-authority-ca-on-ubuntu-20-04
https://kamarada.github.io/en/2018/10/30/how-to-install-website-certificates-on-linux/#.X7Vem64TGR0
https://www.tutorialspoint.com/downloading-files-from-web-using-python
https://stackoverflow.com/questions/63600820/ios-14-self-signed-certificate-not-trustable
http://blog.nashcom.de/nashcomblog.nsf/dx/more-strict-server-certificate-handling-in-ios-13-macos-10.15.htm?opendocument&comments
https://apple.stackexchange.com/questions/371725/why-does-ios-13-not-trust-my-own-root-ca


