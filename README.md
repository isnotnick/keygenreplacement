# keygenreplacement
Implementation of a replacement system for the now-deprecated HTML5 'keygen' tag, and the ActiveX 'CertEnroll' controls.

Keypairs are generated using PKI.js and webcrypto. Stored in browser localstorage. After submission and signing, the signed certificate is 'collected', saved in the same localstorage.
Key, certificate and chain are combined and 'exported' to PKCS#12 (sadly using weak algorithms so that PKCS#12 is compatible with Windows).

Uses the following amazing libraries:
 - PKI.js - https://github.com/PeculiarVentures/PKI.js
 - localForage - https://github.com/localForage/localForage
 - Forge: https://github.com/digitalbazaar/forge
 - PicnicCSS - http://picnicss.com/
