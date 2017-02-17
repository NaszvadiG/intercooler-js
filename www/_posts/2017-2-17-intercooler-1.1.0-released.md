---
layout: blog_post
nav: blog
---

I have released intercooler v1.1.0, available on the main site, as well as through bower and NPM.

  <http://intercoolerjs.org/download.html>


### zepto.js Support!

The biggest change in this release is that we now support [zepto](https://zeptojs.org) as an alternative to jQuery
as a base library.  Zepto + intercooler comes in at ~18kB total, allowing you to build intercooler-based applications
with a smaller javascript infrastructure than [almost all the other major javascript libraries](https://gist.github.com/Restuta/cda69e50a853aa64912d) out there,

Other changes in this release are:

* We respect intercooler response headers even when error response codes are sent to the client (e.g. `X-IC-Redirect` on a 401 response)
* We support a timed value (e.g. "200ms") for the `X-IC-Remove` header, to allow a CSS transition
* We serialize javascript objects used in `ic-include` JSON form, allowing for more complex data to be included in requests
* We now include form values when a form causes a GET
* We now have unit tests running against jQuery v1, v2 and v3
* jQuery 3 is now the documented option

Carson / [@carson_gross](https://twitter.com/carson_gross)