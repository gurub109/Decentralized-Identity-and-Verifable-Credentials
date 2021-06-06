# Why do we need Decentralized Identity (DID) and Verifiable Credentials (VCs)

The initial goal of the Word Wide Web (WWW) was to build the internet, as a decentralized architecture, with open standards so everyone could freely communicate and access information. But the current internet is largely centralized and siloed. The web traffic is controlled by few powerful organization which serves the data through platforms that selectively serve up information based on user's data and thier activity. There is no identity system native to the internet and thus the digital identity is held and controlled through centralized Identity Providers (IdPs). This also resulted in spam, fraud, abuse, misinformation, etc.

The internet is its current form has made it difficult to establish trust with others online, thus leaving the everyday users out of the value chain. Information and data, and the value they create are no longer owned and/or freely accessible by the users.

To fix the above fundamental problem, we need a system that inherently provides [Web of Trust](https://en.wikipedia.org/wiki/Web_of_trust) and allowing the users to control thier identities and to move thier personal data freely from one online system to other without fear of vendor lock-in. 

# Decentralized Identity
Decentralized Identity (DID), also know as "self-sovereign identity" (or SSI) is driven by open web standards at organizations such as W3C, Decentralized Identity Foundation (DIF) and the Hyperledger Project at Linux Foundation.

DIDs are cryptographically secure identifiers that are owned and controlled by a user without a third party Identity Providers (IdPs). It enables the user to prove the ownership of the identity using thier wallet (eg. a mobile device). Using the DID, the user can obtain Verifiable Credentials (VCs) from trusted organizations and, subsequently, present elements of these credentials as proof of claims without the need to authenticate with service providers using usernames and passwords.

DIDs use [Decentralized Public Key Infrastructure (DPKI)](https://github.com/WebOfTrustInfo/rwot1-sf/blob/master/draft-documents/Decentralized-Public-Key-Infrastructure-CURRENT.md) technology by providing identities for people, organizations, and [Internet of things (IoT)](https://en.wikipedia.org/wiki/Internet_of_things). DPKI returns control of online identities (eg. DIDs) to the entities they belong to, bringing the power of cryptography to everyday users by delegating the responsibility of public key management to secure decentralized datastores (blockchains and public databases), so anyone and anything can realize the web of trust.  

## Standards
* [W3C Decentralized Identifiers](https://www.w3.org/TR/did-core/)
* [Decentralized Identity Foundation (DID](https://identity.foundation/)
* [Hyperledger Project at Linux Foundation](https://www.hyperledger.org/use/aries)

# Verifiable Credentials
Identity records are used in everyones daily lives. Driver license is used as evidence to operate a vehicle, education institutions issue diplomas that prove the education qualifications, passports are used to prove the nationality, etc. Verifable Credential (VC) specification defines a model how we could issue, own, store and verify the data over the internat but in a secure manner that respects user's privacy.  

Verifiable Credentials form the foundation for verifiable data in web of trust. They can contain many different type of information as well as different type of credentials. Many software providers, institutions, governments, and businesses are implementing the technology in thier service offerings.

## Standards
* [W3C Verifable Credentials](https://www.w3.org/TR/vc-data-model/)
* [The Verifable Credential Data Model 1.0](https://www.w3.org/TR/vc-data-model/)



## Model
DIDs and VCs typically involves three 
