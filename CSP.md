Content Security Policy (CSP) is a set of policies and headers used to help mitigate against 
cross-site scripting (XSS), clickjacking and other code injection attacks 
resulting from execution of malicious content in the trusted web page context.

It provides a standard method by which to declare the approved origin of content for embeddable objects such as javascript, css, fonts and images. 
Newer types of embeddable content such as web workers are also covered.

## Implementation and usage
Implementation is throiugh the use of http headers
    Subresource Integrity (SRI), to ensure only known, trusted resource files (typically JavaScript, CSS) are loaded from third-party servers (typically CDNs)
    Mixed Content, to clarify the intended browser's policy on pages loaded over HTTPS and linking content over plaintext HTTP
    Upgrade Insecure Requests, hinting browsers on how to handle legacy links on pages migrated to HTTPS
    Credential Management, a unified JavaScript API to access user's credentials to facilitate complex login schemes,
    Referrer Policy, CSP extension to hint the browser on generation of the Referer headers.[18]


## Standard Header
Content-Security-Policy – standard header name proposed by the W3C document. IE 10+ uses a deprecated header to support CSP level 1.


## Complementary Content Security Standards
Subresource Integrity (SRI), to control trust of resources files loaded from 3-party sources (e.g. CDNs hosting common JS frameworks or gogle fonts).

Mixed Content, allows the intended policy for content served over https and http on the same page.

Upgrade Insecure Requests, hinting browsers on how to handle legacy links on pages migrated to HTTPS

Credential Management, a unified JavaScript API to access user's credentials to facilitate complex login schemes,

Referrer Policy, CSP extension to hint the browser on generation of the Referer headers.


## Recommended profiles

## Current Status
As at October 2016 Level 2 is a recommendation of the W3C working group on Web Application Security
https://www.w3.org/TR/CSP2/
Work is underway on level 3 CSP which is expected to supersede Level 2. At time of writing Level 3 has a status of working draft.
https://w3c.github.io/webappsec-csp/

## Browser support
CSP is widely supported by modern web browsers.

CSP 1 is supported by all common browsers from IE11+ (IE11 does not support the standard header, it uses the deprecated  X-Content-Security-Policy header.
https://caniuse.com/#search=csp

CSP level 2 is supported by Firefox, Chrome, Safari, Edge, Opera, Samsung Internet browser. IE11 does not support CSP level 2
