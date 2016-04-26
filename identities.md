# IdentitiesWith a domain or a subdomain in place, an identity for a device or a user can be created.
## Lifecycle### Registration
In order to register a new identity, a certificate must be created beforehand.
An OpenKeyChain certificate for a device or a user is composed of a private key and a public key, just like a certificate for a domain or a subdomain.
The certificate created must be associated with an identity under a domain or a subdomain. A blockchain registration record represents the association.The registratino record is stored on blockchain as a colored coin transaction, and it must be signed by the identity's parent domain or subdomain.### RevocationIn order to revoke an identity created, the domain certificate used to create the identity must be used to create a revocation record on blockchain.

The identity's parent domain or subdomain can revoke the domain on behalf as well.