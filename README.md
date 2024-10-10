# Decentralized Voting Application

## Overview
This project is a decentralized voting application built on the Volta blockchain, provided by Energy Web Chain. The app allows users to securely cast votes and view real-time voting results via a simple user interface. It integrates **React.js**, **Solidity**, **Metamask**, **Hardhat**, and **Ether.js** for seamless blockchain interaction.

## Proposed Methodology

### 1. Technology Stack:
- **Frontend:** React.js is used for building the user interface.
- **Backend:** Solidity is used to create smart contracts on the Ethereum-based Volta blockchain.
- **Blockchain Network:** Volta (Energy Web Chain) for deploying smart contracts.
- **Interaction Tools:**
  - **Metamask:** For interacting with the blockchain.
  - **Hardhat:** Development environment for compiling and deploying smart contracts.
  - **Ether.js:** For connecting the frontend (React) with the smart contracts.

### 2. Smart Contract Design:
- **Voting Contract:**
  - A Solidity contract manages the voting process.
  - **Struct for Candidates:** Stores candidate names and vote counts.
  - **Voting Mechanism:** Users vote by interacting with the smart contract.
  - **Ownership:** The contract owner can add candidates and manage the voting process.
  - **Voting Period:** Set start and end times for voting.
  - **Vote Validation:** Ensures each Ethereum address can vote only once.

### 3. Frontend Design:
- **Login with Metamask:** Users must connect their Metamask wallet to vote.
- **Candidate Display:** Retrieves and shows candidate names and vote counts from the contract.
- **Voting Functionality:** Users can vote for a candidate, and the vote is recorded on the blockchain.
- **User Feedback:** Displays vote confirmation and prevents multiple votes.

### 4. Deployment Process:
1. **Smart Contract:** Written in Solidity and compiled with Hardhat.
2. **Deployment:** The contract is deployed to the Volta blockchain.
3. **Frontend:** React.js interacts with the smart contract via Ether.js.
4. **Transaction:** Metamask signs and sends the user’s vote transaction to the blockchain.

## Results Obtained
- **Successful Contract Deployment:** The smart contract handles candidate registration, voting, and vote counting.
- **Voting:** Users can vote, and votes are immutable and tracked. Voting is restricted to once per address.
- **Real-Time Updates:** Displays real-time candidate vote counts and ensures voting eligibility.
- **User-Friendly Interface:** A clean React.js interface connects the wallet, enables voting, and shows vote status.
- **Account Switching:** Recognizes account changes in Metamask and updates voting eligibility.
- **Voting Time Restriction:** Enforces the voting period, preventing votes outside the timeframe.

## How to Run

### Prerequisites:
- Node.js
- Metamask extension
- Volta blockchain setup

### Steps:

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd <repository-folder>
2. In the .env file in the root folder add your wallet's private key
3. Run "npm install" to install all the dependencies
4. now execute the smart contract using hardhat
5. you will get an address in the terminal output
6. put that address in the .env file, and run the react-app using npm start
7. now login using your metamask wallet and cast your vote!
