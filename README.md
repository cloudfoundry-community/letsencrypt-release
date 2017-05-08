# Let's Encrypt BOSH Release

[Let's Encrypt](https://letsencrypt.org/) is a "free, automated, and open Certificate Authority"
that issues Secure Sockets Layer (SSL) certificates. [BOSH](http://bosh.io/)
is a VM orchestrator that enables the automated deployment of VMs with
pre-existing releases (e.g. "spin me up a VM running nginx at this IP address").

This release enables BOSH deployments to acquire Let's Encrypt SSL certificates.

## This is a Work-in-Progress

This is a work-in-progress; it is non-functional.

Note:
The acme client used here is Daniel Roesler's [acme-tiny](https://github.com/diafygi/acme-tiny/blob/master/acme_tiny.py). Thanks Daniel.

Alternatives:

* [Danny Berger](https://github.com/dpb587) wrote a [Let's Encrypt BOSH
  Release](https://github.com/dpb587/dpb587.me) based on Lukas Schauer's
  [dehydrated](https://github.com/lukas2511/dehydrated) Let's Encrypt client.

* [Lyle Franklin](https://github.com/ljfranklin) crafted a Concourse CI
  [pipeline](https://github.com/ljfranklin/deployments/blob/master/ci/setup-env/pipeline.yml#L111-L113) that uses Let's Encrypt's DNS challenge to obtain an SSL
  certificate.
