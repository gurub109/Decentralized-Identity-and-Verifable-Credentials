# Microsoft Verifiable Credential Service
Azure AD verifiable credentials service is currently in public preview. Microsoft is actively colloborating with members of [Decentralized Identity Foundation](https://identity.foundation/), the [W3C Credentials Community Group](https://www.w3.org/TR/did-core/), and the wider identity community to unlock a new set of experiences for users and organizations to control thier self-soverign identity (SSI).

## How does Microsoft Verifiable Credential Service works
To deliver Web of Trust model, Microsoft implemented following key components:

![image](https://docs.microsoft.com/en-us/azure/active-directory/verifiable-credentials/media/decentralized-identifier-overview/microsoft-did-system.png)

* **Decentralized Repository** 
    * ION (Identity Overlay Network) is a Layer 2 open, permissionless network based on the purely deterministic Sidetree protocol, which requires no special tokens, trusted validators, or other consensus mechanisms; the linear progression of Bitcoin's time chain is all that's required for its operation
    * Microsoft manages thier own ION node
    * Microsoft [open sourced a npm package](https://www.npmjs.com/package/@decentralized-identity/ion-tools) to make working with ION network easy to integrate into apps and services. The open source libraries include creating a new DID, generating keys, and anchoring DID on the Bitcoin blockchain
* **User Agent/Wallet**
   * Microsoft Authenticator App on both iOS and Andriod mobile platform is extended to support Decentralized Identities (DIDs) and Verifiable Credentials (VCs)
   * Authenticator creates DIDs, facilitates issuance and presentation requests for verifiable credentials and manages the backup of DID's seed through an encrypted wallet file
* **Microsoft Resolver**
   * Provides API that connects to Microsoft ION node to look up and resolve DIDs using the did:ion method and return the DID Document Object (DDO). he DDO includes DPKI metadata associated with the DID such as public keys and service endpoints
* **Azure Active Directory Verified Credential Service**
   * Provides an issuance and verification API and open-source SDK for W3C Verifiable Credentials that are signed with the did:ion method
   * It enables identity owners to generate, present, and verify claims which enables the trust between users of the systems       
