# Charity - Decentralized Donation Platform

Decentralized donation platform is designed to make charitable contributions more transparent and accessible using blockchain technology. The application allows users to allocate donations across different countries, track their donation amounts, and submit XRP transactions through the XRP Ledger (XRPL) testnet.

The project also integrates Sismo Connect for identity verification using zero-knowledge proofs.

## Features

- **Wallet Connection:** Connect an XRP Ledger wallet using its seed.
- **Identity Verification:** Integrate Sismo Connect for verification using supported authentication methods.
- **Country-Based Donations:** Select countries and specify the amount of XRP to donate.
- **Blockchain Transactions:** Submit XRP payment transactions to predefined destination wallets on the XRPL testnet.
- **Donation Tracking:** View pledged donation amounts and donation progress.
- **Transaction Receipts:** Display transaction identifiers (TXIDs) for submitted donations.
- **Wallet Balance:** Retrieve and display the connected wallet's XRP balance.
- **Donation Management:** Reset donation selections and review donation status.

## Supported Countries

The current implementation includes donation destinations for:

- Singapore
- Canada
- Brazil
- France
- Australia
- Iceland
- Japan
- United States

## Technologies Used

| Technology | Purpose |
|---|---|
| React.js | Frontend user interface |
| JavaScript | Application logic and state management |
| TypeScript | Used in the header component |
| XRP Ledger (`xrpl`) | Wallet interaction and XRP transactions |
| Sismo Connect | Identity verification |
| React Bootstrap | UI components and progress bars |
| Material UI | Buttons and input fields |
| React Icons | Icons and visual elements |
| CSS | Styling and layout |

## Project Structure

```text
CharityDAO/
├── src/
│   ├── App.js
│   ├── AppContext.js
│   ├── GatedContent.js
│   ├── Header.tsx
│   ├── VoteOption.js
│   ├── index.js
│   └── countryAddresses.txt
├── .gitignore
└── README.md
```

*Note: This is a simplified representation of the source files. Ensure that all required stylesheets, images, components, and project configuration files are included in the complete repository.*

## Prerequisites

Before running the project, ensure that you have:

- Node.js and npm installed.
- A compatible XRP Ledger testnet wallet.
- Access to the XRPL testnet.
- The required Sismo Connect configuration.
- The project's complete source files and a valid `package.json`.

## Installation and Setup

### 1. Clone the repository

Replace `YOUR-USERNAME` with your GitHub username.

```bash
git clone https://github.com/YOUR-USERNAME/CharityDAO.git
cd CharityDAO
```

### 2. Install dependencies

Once the project's `package.json` is available, run:

```bash
npm install
```

### 3. Configure the application

Verify the XRPL testnet endpoint and Sismo Connect configuration. Ensure that wallet credentials and other sensitive values are not hardcoded in the source code.

### 4. Start the development server

For a Create React App project, run:

```bash
npm start
```

The development server will typically be available at:

http://localhost:3000

*The uploaded project archive does not contain a `package.json` or all the referenced application assets, so these setup commands require the complete project files before the application can run successfully.*

## How to Use

1. Launch the application in your browser.
2. Complete the supported identity verification flow.
3. Connect an appropriate XRP Ledger testnet wallet.
4. Select a country for your donation.
5. Enter the amount of XRP you want to pledge.
6. Submit your donation selection.
7. Confirm the donation transaction.
8. Review the transaction status and available receipt information.

## Blockchain Integration

CharityDAO uses the XRP Ledger JavaScript library to interact with the XRPL testnet.

The application prepares, signs, and submits XRP payment transactions to predefined country-specific destination addresses.

Transactions are intended for **testnet use only**. Testnet XRP is not equivalent to real-world XRP and should not be used to represent production charitable payments.

## Security Considerations

- Never commit wallet seed phrases, private keys, API secrets, or other credentials to GitHub.
- Remove sensitive credentials from tracked files and rotate any exposed wallet credentials before using the project further.
- Use dedicated testnet wallets for development.
- Do not use this prototype to handle real donations without a security review.
- Validate transaction outcomes and verify payment status before reporting a donation as successful.
- Store sensitive configuration in appropriate environment variables and keep local environment files out of version control.

## Current Limitations

- The application is configured to use the XRPL testnet.
- Donation destinations are predefined in the application.
- Donation progress and voting data are primarily managed in frontend state.
- Persistent donation history and a production-grade administrative dashboard are not established by the reviewed source files.
- Identity verification, wallet connection, and transaction confirmation require further testing before production deployment.

## Future Enhancements

- Integrate a secure backend and persistent donation database.
- Provide an auditable donation history.
- Improve transaction confirmation and error handling.
- Add charity registration and destination verification.
- Introduce governance-based voting and transparent fund allocation.
- Add automated testing, monitoring, and production deployment support.

## Contributing

Contributions and suggestions are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Push the branch to your fork.
5. Open a pull request describing your changes.

## Disclaimer

CharityDAO is an educational and development project exploring blockchain-based charitable donations. It is not a production-ready financial service. Always verify transaction details and use testnet credentials during development.

## License

A license has not yet been specified. Add an appropriate open-source license before inviting others to reuse or distribute the project.
