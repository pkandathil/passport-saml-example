# passport-saml-example

This node.js web application demonstrates SSO authentication provided by RIT's Shibboleth Server (https://shibboleth.main.ad.rit.edu/), using the `passport-saml` package.

Config
======

This app requires 3 files to be placed in the project's root directory. These files include (1) the public key of the Identity Provider (IdP). In this case, RIT's Shibboleth Server is the IdP. As a Service Provider (SP), you need to generate your own (2) public key and (3) private key. These files are named as follows:

- `cert.pem`: SP's public key (Generated by you)
- `cert_idp.pem`: IdP's public key (RIT's is contained in https://shibboleth.main.ad.rit.edu/rit-metadata.xml)
- `key.pem`: SP's private key (Generated by you)

Usage
=====

```
npm install
node app.js
```
