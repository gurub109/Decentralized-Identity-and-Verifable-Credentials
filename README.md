# Why do we need Decentralized Identity (DID) and Verifiable Credentials (VCs)

The initial goal of the [Word Wide Web (WWW)](https://en.wikipedia.org/wiki/World_Wide_Web) was to build the internet as a decentralized architecture platform, with open standards so everyone could freely communicate and access information. But the current internet is largely centralized and siloed. The web traffic is controlled by few powerful organizations which provides the data through platforms that selectively serves the information based on user's data and their activity. There is no identity system native to the internet and thus the digital identity is held and controlled through their own centralized Identity Provider (IdP) systems. This resulted in spam, fraud, abuse, misinformation, etc.

The internet in its current form has made it difficult to establish trust with others online, thus leaving the everyday users out of the value chain. Information and data, and the value they create are no longer owned and/or freely accessible by the users.

To fix the above fundamental problem, we need a system that inherently provides [Web of Trust](https://en.wikipedia.org/wiki/Web_of_trust) and allowing the users to control their identities and to move their personal data freely from one online system to other without fear of vendor lock-in. 

# Decentralized Identity
Decentralized Identifier (DID), also know as "self-sovereign identity" (or SSI) is driven by open web standards at organizations such as W3C, Decentralized Identity Foundation (DIF) and the Hyperledger Project at Linux Foundation.

DIDs are cryptographically secure identifiers that are owned and controlled by a user without a third-party Identity Providers (IdPs). It enables the user to prove the ownership of the identity using thier wallet (e.g., a mobile device). With their DID, the user can obtain Verifiable Credentials (VCs) from trusted organizations and, subsequently, present elements of these credentials as proof of claims without the need to authenticate with service providers using usernames and passwords.

DIDs use [Decentralized Public Key Infrastructure (DPKI)](https://github.com/WebOfTrustInfo/rwot1-sf/blob/master/draft-documents/Decentralized-Public-Key-Infrastructure-CURRENT.md) technology by providing identities for entities (people, organizations, and [Internet of things (IoT)](https://en.wikipedia.org/wiki/Internet_of_things)). DPKI returns control of identities to the entities they belong to, bringing the power of cryptography to everyday users by delegating the responsibility of public key management to secure decentralized datastores ([blockchains](https://en.wikipedia.org/wiki/Blockchain) and public databases), so anyone and anything can realize the web of trust.  
  
## Standards
* [W3C Decentralized Identifiers](https://www.w3.org/TR/did-core/)
* [Decentralized Identity Foundation (DID)](https://identity.foundation/)
* [Hyperledger Project at Linux Foundation](https://www.hyperledger.org/use/aries)

# Verifiable Credentials
Identity records are used in everyone's daily lives. Driver license is used as evidence to operate a vehicle, education institutions issue diplomas that prove the education qualifications, passports are used to prove the nationality, etc. Verifiable Credential (VC) specification defines a model on how we could issue, own, store and verify the data over the internet but in a secure manner that respects user's privacy.  

Verifiable Credentials form the foundation for verifiable data in web of trust. They can contain many different types of information as well as different types of credentials. Many software providers, institutions, governments, and businesses are implementing the technology in their service offerings.

## Popular Use Cases
* Education
  * Digital transcripts
  * Online class attendance and completion status   
* Retail
  * Address verification
  * Fraud detection 
* Finance
  * Reuse KYC (Know Your Customer)
  * Money transfer 
* Healthcare
  * Prescription
  * Medical records (vaccination, traveling illness, etc.) 

## Standards
* [W3C Verifiable Credentials](https://www.w3.org/TR/vc-data-model/)


# Building a Trust Model
A web of trust typically involves the following roles:
* **Subject** an entity about which verifiable credentials (attested claims) are made
* **Holder** an entity that holds one or more verifiable credentials in their wallet and also generates verifiable presentations for the verifiers. Holder is typically the **subject** but in cases such as minor (**subject**), the verifiable credentials are held by parent or guardian (**holder**)
* **Issuer** an entity that asserts the claims about **subject(s)** by creating a verifiable credential from the claims and then transmits them to a holder
* **Verifier** an entity (relying party) that receives the verifiable credentials (presentations) from a **holder** and verifies the claims asserted by the **issuer** without their knowledge or interaction
* **Verifiable data registry** a system that mediates the creation and verification of identifiers, public keys, verifiable credential schemas, revocation registries, etc. A [blockchain](https://en.wikipedia.org/wiki/Blockchain) or public database is typically used as registry and verifiable credentials (asserted claims) are never stored in the registry

### Roles and information flows
![image](https://user-images.githubusercontent.com/26188338/120909336-4cda3c80-c631-11eb-8881-cc3422a5f623.png "Roles and information flows")

# Wallets and Agents
Web of trust model is built on self-certifying identifiers and user-centric cryptography. The role of the user (**holder**) is central to the ecosystem and offers greater sovereignty of their own information and empowerment to manage their digital identity and personal information through new class of software known as **digital wallets**.

Digital wallets are applications that allow an end user to manage their digital credentials and associated cryptographic keys. They allow **holders** to prove identity related information about **subject(s)** by sharing a selective disclosure of attributes of the verifiable credentials in a privacy-preserving manner.

The concept of wallet can be further identified as a simple Wallet or Agent. The role of a wallet is to store keys, credentials, and secrets. An agent is a software that controls access to a wallet and other storage, which can live in different locations on a network (cloud vs local). The role of an agent is complex and includes messaging or interaction with other agents in the decentralized ecosystem.



