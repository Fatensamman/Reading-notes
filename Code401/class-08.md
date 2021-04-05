##  Access Control (ACL)

- When is Basic Authorization used vs. Bearer Authorization?

The Basic and Digest authentication schemes are dedicated to the authentication using a username and a secret. The Bearer authentication scheme is dedicated to authentication using an OAuth2 token. JWT authentication is the best choice as it is a token, but nothing prevents you from using a custom scheme.

- What does the JSON Web Token package do?

JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair. This information can be verified and trusted because it is digitally signed.

- What considerations should we make when creating and storing a SECRET?

Secrets that you create in Secrets Manager can be static or dynamic in nature. Dynamic secrets have their expiration date and time enforced when secret data is read or accessed.

## Term:

- Encryption is the act of transforming data into a coded code that masks the true nature of the data. Cryptography is the science of encrypting and decrypting knowledge. Unencrypted data is referred to as plaintext in programming, while encrypted data is referred to as ciphertext.

- A token is a component of a two-factor authentication protection system that can be used to grant access to computer services. Software tokens can be duplicated and placed on a general-purpose computing device like a personal computer, notebook, PDA, or cell phone.

- bearer :The Bearer authentication scheme is dedicated to the authentication using a token. Even if this scheme comes from an OAuth2 specification, you can still use it in any other context where tokens are exchange between a client and a server.

- The secret is to Secrets generated in Secrets Manager can be either static or dynamic. The expiration date and time of a static secret are set at the time of creation or rotation. When a complex hidden's secret data is read or downloaded, the expiration date and time are enforced.

- JSON Web Token is a lightweight and self-contained mechanism for safely sharing information as a JSON entity between parties. Since it is digitally signed, this information can be checked and trusted. JWTs may be signed with a password (using the HMAC algorithm) or with an RSA or ECDSA public/private key pair.

## Preview

**Role Based Access Control** : RBAC is the concept of granting users machine access depending on their role within an enterprise. Users are divided into positions based on general job tasks and machine access requirements, and the system needs of a particular workforce are assessed. Each individual is then given access based solely on their job assignment. Access management gets even simpler as each role's access criteria are strictly pursued.

![image](https://docs.oracle.com/cd/E65459_01/admin.1112/e65449/content/images/admin/rbac/rbac_overview.png)

#### sources
[toterial](https://www.youtube.com/watch?v=C4NP8Eon3cA)
[general Rbac](https://docs.oracle.com/cd/E65459_01/admin.1112/e65449/content/general_rbac.html)
