# The Internet Computer Protocol Handbook [WiP]

Welcome. This is EasyA's legendary handbook. If you want to learn Internet Computer Protocol (ICP) like a legend, then you're in the right place.

# Purpose

This handbook serves as a guide to the Internet Computer Protocol ecosystem, geared towards those just joining for the first time. It isn't just a beginners' handbook; it's a legendary handbook. Even if you've already immersed yourself in the ecosystem, you'll find tons of helpful tidbits around here!

# The EasyA App

Of course, the best place to start is always the [EasyA](https://www.easya.io) app! Download it here for the fastest and most fun way to learn about ICP. Download it directly right [here](https://links.easya.io/links/gotoapp)!

## Table of Contents

- [Introduction](#introduction)
- [Getting Started](#getting-started)
- [Core Concepts](#core-concepts)
- [Development Tools](#development-tools)
- [Smart Contracts](#smart-contracts)
- [ICP Network](#icp-network)
- [Ecosystem Projects](#ecosystem-projects)
- [Resources](#resources)
- [Handy Code Snippets](#handy-code-snippets)
- [Contributing](#contributing)

## Introduction

What is Internet Computer Protocol:

- [Internet Computer Website](https://internetcomputer.org/) - The official website providing comprehensive information about ICP.
- [Internet Computer Whitepaper](https://internetcomputer.org/whitepaper.pdf) - The technical whitepaper explaining ICP's architecture and design principles.

## Getting Started

The no-fluff starter:

- [Internet Computer Developer Hub](https://internetcomputer.org/docs/current/home) - The main entry point to documentation, guides, and references.
- [Your First dApp](https://internetcomputer.org/docs/current/developer-docs/quickstart/hello10mins) - Tutorial on deploying your first decentralized app in 10 minutes.

## Core Concepts

Explanation of fundamental concepts in the ICP ecosystem:

- [ICP Architecture](https://internetcomputer.org/how-it-works) - Learn how ICP realizes the vision of the Internet Computer.
- [Candid](https://github.com/dfinity/candid) - The interface description language for ICP.

## Development Tools

Key tools and environments for ICP:

- [dfx](https://github.com/dfinity/sdk) - Command-line tool to interact with the IC written in Rust.
- [Motoko Playground](https://m7sm4-2iaaa-aaaab-qabra-cai.ic0.app/) - An online playground environment for Motoko, ICP's native programming language.

## Smart Contracts

How to write and deploy smart contracts on ICP:

- [Motoko](https://github.com/dfinity/motoko) - The home of the Motoko language, designed for writing smart contracts on ICP.
- [Rust CDK](https://github.com/dfinity/cdk-rs) - Canister Development Kit for Rust on ICP.

## ICP Network

Going into the network level:

- [Network Status](https://dashboard.internetcomputer.org/) - Live stats and explorer for the ICP network.
- [NNS Dapp](https://nns.ic0.app/) - Web interface for interacting with the Network Nervous System.

## Ecosystem Projects

Cool projects built on ICP:

- [Internet Identity](https://github.com/dfinity/internet-identity) - Pseudonymous authentication system for ICP.
- [OpenChat](https://github.com/open-ic/open-chat) - An open chat app built on ICP.

## Resources

Extra stuff:

- [DFINITY Developer Forum](https://forum.dfinity.org/) - Main forum about the Internet Computer.
- [Internet Computer Wiki](https://wiki.internetcomputer.org/wiki/Internet_Computer_wiki) - General knowledge resource about the Internet Computer.

## Handy Code Snippets

Get a taste of ICP development with these code snippets:

### Hello World in Motoko

```motoko
actor {
  public func greet(name : Text) : async Text {
    return "Hello, " # name # "!";
  };
};
```

### Calling a Canister Function

```javascript
import { Actor, HttpAgent } from "@dfinity/agent";
import { idlFactory } from "./declarations/hello";

const agent = new HttpAgent();
const hello = Actor.createActor(idlFactory, { agent });

const greeting = await hello.greet("World");
console.log(greeting);
```

These examples showcase:
1. A simple Motoko actor that implements a greeting function.
2. How to call a canister function using the JavaScript agent.

## Contributing

We welcome contributions to make this handbook even more legendary! Here's how you can contribute:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/amazing-addition`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add some amazing feature'`)
5. Push to the branch (`git push origin feature/amazing-addition`)
6. Create a new Pull Request

Please ensure your contributions align with our code of conduct and contribution guidelines.

## Credit/Inspiration

This handbook was inspired by the famous awesome lists by sindresorhus and the Awesome Internet Computer list. We need awesome lists for Web3 ecosystems, with more of a hacker's guide to how they work. This is the answer to that need.
