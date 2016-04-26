# Introduction

The proliferation of cryptographic protocols such as Transport Layer Security (TLS) transformed the concept of security on internet from a luxury affored by few into a commodity. With TLS, an average internet user is able to exchange encrypted messages online, use credit cards online, or download files; all without the fear of censorship or compromising his or her computer system.
However, TLS's usefulness is limited outside the boundaries of simple but familiar server-client architectures.
With SSL certificates, it is possible to protect users by providing identities to service providers and ways for users to authenticate them. However, as more and more devices and services are going online. authenticating only service providers is simply not enough; the days of only servers with identities are over, as every user, every device needs a certificate of its own.We need identities for not only social network services, but digital door locks, refrigerators, and automobiles. We also need new ways for devices and services to identify and authenticate each other without human interactions.
Simply put, existing Public Key Infrastructure (PKI) for providing identities to web services is not good enough. Even Google is developing new technologies such as Certificate Transparency[^1] to supplement the shortcomings of the PKI technologies.
Most of limitations of PKI systems come from the centralized nature of PKI providers, and distributed ledger technologies such as blockchain are expected to play a huge role in supplementing and replacing the limited PKI systems[^2].
Blocko's OpenKeyChain is intended to be a robust real life implementation of such a PKI system based on blockchain technology
OpenKeyChain enables developers and users to deploy new PKIs without huge investments by leveraging the existing public blockchain infrastructure; anyone can register and manage certificates for devices and services, and sign or encrypt messages between parties even without TLS involved.
OpenKeyChain is an open standard allowing others to review and extend its ideas. Blocko's Coinstack SDKs include reference implementations of OpenKeyChain; applications on all platforms (servers, clients, and web browers) are supported.
[^1]: https://www.certificate-transparency.org/[^2]: https://en.wikipedia.org/wiki/Public_key_infrastructure#Blockchain-based_PKI