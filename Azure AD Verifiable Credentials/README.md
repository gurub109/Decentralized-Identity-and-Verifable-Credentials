# Microsoft Verifiable Credential Service
Azure AD verifiable credentials service is currently in public preview. Microsoft is actively colloborating with members of [Decentralized Identity Foundation](https://identity.foundation/), the [W3C Credentials Community Group](https://www.w3.org/TR/did-core/), and the wider identity community to unlock a new set of experiences for users and organizations to control thier self-soverign identity (SSI).

## How does Microsoft Verifiable Credential Service works
To deliver Web of Trust model, Microsoft implemented following key components:

![image](https://docs.microsoft.com/en-us/azure/active-directory/verifiable-credentials/media/decentralized-identifier-overview/microsoft-did-system.png)

* **Decentralized Repository** 
    * ION (Identity Overlay Network) is a Layer 2 open, permissionless network based on the purely deterministic Sidetree protocol, which requires no special tokens, trusted validators, or other consensus mechanisms; the linear progression of Bitcoin's time chain is all that's required for its operation
    * Microsoft [open sourced a npm package](https://www.npmjs.com/package/@decentralized-identity/ion-tools) to make working with ION network easy to integrate into apps and services.  
