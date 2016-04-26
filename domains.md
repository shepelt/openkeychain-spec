# Domains

In order to manage identities using OpenKeyChain, a root domain needs to be created first.

A root domain is a logical equivalent of an individual PKI. Certificates issued under a domain are not compatible with certificates issued under different domains.

Usually, a single domain represents a single organization or an application.## RepresentationEach domain is a logical entity; domains and certificates are represented similarily under blockchain.
### Domain Organization
Under each domain, other domains and certificates reside.

A domain with a parent as another domain is called a "subdomain." A domain with a child is called a "parent domain."A domain without any parent is called a "root domain."## Lifecycle### Registration
In order to create a domain, a domain certificate needs to be created.

An OpenKeyChain certificate is composed of a private key and a public key pair, using elliptic curve cryptography with secp256k1[^1] curve.The certificate created is associated with a domain through a registration record on blockchain.
A registration record is represented as a transaction using OpenKeyChain colored coin[^2] protocol. The registration record must  conform to OpenKeyChain colored coin standards in order to be recognized as one.### Revocation
In order to revoke a domain created, the domain certificate used to create the domain must be used to create a revocation record on blockchain.

If the domain has a parent domain, the parent domain can revoke the domain on behalf of the domain being revoked.[^1]: http://www.secg.org/sec2-v2.pdf, https://en.bitcoin.it/wiki/Secp256k1[^2]: https://en.bitcoin.it/wiki/Colored_Coins