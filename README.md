Having trouble getting the old howdykolache.com site to redirect to howdybreakfastbuns.com for SSL/TLS.

non http howdykolache -> howdybreakfastbuns.com works

https howdykolache hangs indefinitely.

I think this is because the https / SSL / TLS negotiation is failing so it hangs and therefore the redirect never happens.

The redirect is happening via a DNS redirect record at namecheap, so I would have thought that the redirect happens BEFORE
the SSL negotiation, but I'm not observing that behavior.

So instead, this repository is here solely to create a single page to publish on netlify, where it will successfully complete
the https negotiation, then serve a static page. That page just contains a javascript directive to redirect the site.

This will probably be worse for SEO.

https://blog.dnsimple.com/2016/08/https-redirects/
