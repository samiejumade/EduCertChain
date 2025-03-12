

# BlockChain Based Documents Verification System With-IPFS

This project aims to create a secure and decentralized system for document verification using Blockchain and InterPlanetary File System (IPFS) technologies. The system stores the hash of the documents in the Blockchain network and the documents themselves in the IPFS network. This ensures that the documents cannot be tampered with or altered, and they can be easily retrieved and verified by authorized parties.

## Features

- Secure documents verification using Blockchain and IPFS technologies
- Decentralized system, with no central authority or single point of failure
- Fast and easy verification process, with no need for intermediaries or third-party services
- User-friendly interface for document upload and verification
- Support for multiple document types and formats

## Requirements

- Node.js and npm installed on your system
- Ganache or any other Ethereum network client
- IPFS client (optional)

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
```

2. Install dependencies:
```bash
cd EduCertChain 
npm install
```

3. Start local Hardhat node:
```bash
npx hardhat node
```

4. Deploy smart contract:
```bash
npx hardhat run scripts/deploy.js --network localhost
```

5. Update contract address in js/verify.js and js/App.js with the deployed contract address

6. Install IPFS desktop application from https://ipfs.tech/#install

7. Start IPFS desktop

8. Open the application using Live Server extension in VS Code

## Usage

1. The owner of the system must first add an exporter to the list of authorized parties. This is done by clicking on the "Add Exporter" button and entering the exporter's Ethereum address.
2. Upload a document to the system by clicking on the "Upload Document" button and selecting a file from your computer. The document will be encrypted and stored in the IPFS network, and its hash will be recorded in the Blockchain.
3. Verify a document by clicking on the "Verify Document" button and entering its unique identifier (hash) in the input field. The system will retrieve the document from the IPFS network, decrypt it, and compare its hash with the one recorded in the Blockchain.
4. The system will display a message indicating whether the document is authentic or not.

Thank you for using our system!
