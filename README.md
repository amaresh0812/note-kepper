# dkeeper

Welcome to your new dkeeper project and the Internet Computer development community! This README provides a detailed overview designed to help you—and anyone new to this repository—get started efficiently and with confidence, regardless of prior Web3 experience.

## About This Project

This dkeeper project is built as an introduction to decentralized app development using Motoko and Internet Computer (IC) technologies. The project originated from a guided learning experience with Dr. Angela Yu, a Lead Udemy Instructor. Through her mentorship, this repository represents not just a technical milestone, but also a personal journey—exploring the core principles of Web3, Motoko, and the wider IC ecosystem.

## Project Structure & Getting Started

You’ll find that your project directory comes preloaded with template files and a default configuration to speed up development. Editing these templates and incorporating your own logic is encouraged.

To explore and modify the project, start by examining:

- The directory structure.
- The default configuration files.
- Main source code and canister setup.

**Pro Tip:** Any changes in your development environment will not impact production deployments or your identity tokens.

## Essential Development Commands

To help you get working right away, here are the most important commands and procedures:

```bash
cd dkeeper/
dfx help             # View the DFINITY command line help
dfx config --help    # Learn how to manage your config
```

### Running the Project Locally

Spin up your local replica and deploy the project canisters with:

```bash
# Starts the replica, running in the background
dfx start --background

# Deploys your canisters to the replica and generates your candid interface
dfx deploy
```

Your application will then be accessible at:
`http://localhost:8000?canisterId={asset_canister_id}`

If working on the frontend, start the dev server:

```bash
npm start
```

This launches a server at `http://localhost:8080`, proxying API calls to the backend replica at port 8000.

## Frontend Environment Variables Reminder

If hosting your frontend outside DFX, you may need to:

- Set `NODE_ENV` to `production` (for Webpack users).
- Customize `process.env.NODE_ENV` in generated declarations.
- Write a custom `createActor` constructor for your application’s needs.

## Recommended Documentation

Explore official docs to deepen your Motoko, IC, and JavaScript development understanding:

- Quick Start (DFINITY): sdk.dfinity.org/docs/quickstart/quickstart-intro.html
- SDK Developer Tools: sdk.dfinity.org/docs/developers-guide/sdk-guide.html
- Motoko Language Guide: sdk.dfinity.org/docs/language-guide/motoko.html
- Motoko Quick Reference: sdk.dfinity.org/docs/language-guide/language-manual.html
- JavaScript API Reference: erxue-5aaaa-aaaab-qaagq-cai.raw.ic0.app

## Acknowledgments

- Special thanks to **Dr. Angela Yu** for expert guidance and encouragement throughout this learning journey.
- Gratitude to the Udemy and DFINITY communities for their support and resources.

*This README aims to make onboarding as clear and thorough as possible, helping both you and future collaborators feel welcome and empowered to contribute!*
