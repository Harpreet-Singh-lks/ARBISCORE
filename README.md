## ARBISCORE 


This is an on chain AI agent that generates credit scores for our lending protocol and we also have an API that can be used for other projects as well 

This project is a smart contract written in Rust using the Stylus SDK, which allows developers to write Ethereum-compatible smart contracts in Rust and compile them to WebAssembly (WASM). The contract is designed to be ABI-compatible with Solidity, meaning it can be called from both Solidity and Rust, making it highly versatile.

The contract implements a Q-learning algorithm for a lending protocol. Q-learning is a reinforcement learning technique used to optimize decision-making in dynamic environments. In this case, the algorithm is applied to a lending protocol to optimize decisions such as:

Whether to approve a loan.

How much credit to extend to a user.

When to liquidate a loan.

The project also includes a Rust script (counter.rs) that demonstrates how to interact with the deployed contract using the ethers-rs library, which is a popular Rust library for Ethereum development.

Key Features
Rust-Based Smart Contract:

The contract is written in Rust, which is known for its performance, safety, and modern features.

It uses the Stylus SDK to ensure compatibility with Ethereum and other EVM-based blockchains.

Q-Learning Algorithm:

The contract implements a Q-learning algorithm, a type of reinforcement learning used to make optimal decisions in a dynamic environment.

The algorithm learns from user behavior (e.g., loan repayment history, interactions) to optimize lending decisions.

ABI Compatibility:

The contract is ABI-compatible with Solidity, meaning it can be called from both Solidity and Rust.

This makes it easy to integrate with existing Ethereum tools and workflows.

Persistent Storage:

The contract uses persistent storage to store key data such as:

The Q-table (used for Q-learning).

User states (e.g., loan history, repayment ratios).

User credit scores.

Events:

The contract emits events to notify external applications about key actions, such as:

Updates to the Q-table.

Computed credit scores for users.

Interoperability:

The project includes a Rust script (counter.rs) to demonstrate how to interact with the contract using the ethers-rs library.

This script can be used to call contract functions, send transactions, and read state variables.
