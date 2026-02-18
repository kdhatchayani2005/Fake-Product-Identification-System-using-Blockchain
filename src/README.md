# Fake Product Identification System using Blockchain

The **Fake Product Identification System using Blockchain** is a decentralized application developed to detect and prevent counterfeit products in the market. In this system, manufacturers register product details such as product ID, batch number, and production information on the blockchain using smart contracts. Each product is linked with a unique QR code or identification number that consumers can use to verify authenticity. Since blockchain technology is immutable and tamper-proof, once the product information is stored, it cannot be altered or manipulated. This ensures transparency, security, and trust between manufacturers and consumers, helping to reduce fake products and protect brand reputation.

```
NOTE: Devlopement of this project has been stopped because I am working on newer projects so this repository will not be receving any updates.
Last Update: Fixed issues with connecting with metamask.
```

### Blockchain based Fake product identification Solution using QR Codes

## Installation & Demo
[![FraudBlock](https://github.com/kdhatchayani2005/Fake-Product-Identification-System-using-Blockchain/blob/main/project%20output%20screenshots/Screenshot-1.png)]

## Packages Required:-
- Truffle v5.6.7 (core: 5.6.7)
- Ganache v7.5.0
- Solidity v0.5.16 (solc-js)
- Node v16.20.0
- Web3.js v1.7.4
- npm 7.5.1

## Other Requirements:-
1. Any chromium based browser i.e. Chrome 
2. Metamask browser extension
    
## Setup Process 

1. Clone the project
```
git clone https://github.com/kdhatchayani2005/Fake-Product-Identification-System-using-Blockchain
```
2. Go to the project folder, open terminal there and run following command to install required node_modules:-
```
npm install
```
3. Compile contract source files. (Compilation and deployment can be done using truffle migrate):-
```
truffle compile
```
4. Open Ganache, (to setup local blockchain)
    - crerate new workspace
    - add truffle-config.js  in truffle project 
    - change port to 7545 in server settings (same as port in truffle-config.js)
5. In chrome, open metamask 
   - add new test network using  
        - NETWORK ID (i.e. 5777 ,from Ganache Server settings) 
        - RPC SERVER (i.e HTTP://127.0.0.1:7545 ,from Ganache Server settings)
        - CHAIN CODE (i.e. 1337)
   - import account using private key of any account from local blockchain available in Ganache.
6. In terminal, run following commands:-
- Run migrations to deploy contracts.
```
truffle migrate
```

- To start a server and it will open a homepage (index.html) file in the default browser.
```
npm run dev 
``` 
7. Login to metamask ,and connect the added account to local blockchain by clicking the 'Connect Wallet' button on the homescreen.
8. Interact with website
