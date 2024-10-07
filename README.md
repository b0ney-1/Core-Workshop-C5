# Metaschool x Core [ Shobhit University]

Welcome❕ 🚀This README provides essential information and resources for setting up the project.
- [Metaschool Official Website](https://metaschool.so/)
- [What are we building](https://metaschool.so/courses/build-decentralized-social-media-dapp-on-core)

## Table of Contents

1. [Installing Pre-requisites](#installing-pre-requisites)
2. [Setting up Metamask](#setting-up-metamask)
3. [Setting up the Project](#setting-up-the-project)
4. [Configuring the Project](#configuring-the-project)
5. [Project Deployment](#project-deployment)
6. [Contract Verification](#contract-verification)
7. [Create Pull Request](#create-pull-request)

## Installing Pre-requisites

### 1. Installing Node.js and Git

To install Node.js and Git on Ubuntu-based systems, follow these steps:

1. Open a terminal window.

2. Update your package list:
   ```
   sudo apt update
   ```

3. Install Node.js and npm (Node Package Manager):
   ```
   sudo apt install nodejs npm
   ```

4. Verify the installation:
   ```
   node --version
   npm --version
   ```

5. Install Git:
   ```
   sudo apt install git
   ```

6. Verify the Git installation:
   ```
   git --version
   ```

### 2. Creating a GitHub Account and Setting Up Two-Factor Authentication

1. Go to [GitHub's website](https://github.com/) and click on "Sign up".

2. Fill in your details (username, email, and password) and complete the sign-up process.

3. Once your account is created, go to your account settings by clicking on your profile picture in the top-right corner and selecting "Settings".

4. In the left sidebar, click on "Password and authentication".

5. Scroll down to the "Two-factor authentication" section and click "Enable two-factor authentication".

6. Choose your preferred method:
   - For app-based authentication (recommended):
     - Download Google Authenticator or Microsoft Authenticator on your smartphone.
     - Follow the on-screen instructions to set up the authenticator app with your GitHub account.

   - For SMS authentication:
     - Choose the SMS option and enter your phone number.
     - Follow the prompts to complete the setup.

7. Save your recovery codes in a safe place. These will help you regain access to your account if you lose your authentication device.

8. Once set up, you'll need to enter a code from your authenticator app or SMS each time you log in to GitHub.

With these steps completed, you'll have the necessary tools installed on your system and a secure GitHub account ready for collaboration.

## Setting up Metamask

### 1. Installing Metamask

1. Go to the [Metamask website](https://metamask.io/).
2. Click on "Download" and select your browser (Chrome, Firefox, Brave, or Edge).
3. You'll be redirected to your browser's extension store. Click "Add to Chrome" (or your respective browser).
4. Once installed, click on the Metamask icon in your browser's extension area to begin setup.

### 2. Setting up your Metamask Wallet

1. Click "Get Started" on the Metamask welcome page.
2. Choose "Create a new wallet" if you're new to Metamask, or "Import an existing wallet" if you have one.
3. Create a strong password for your wallet.
4. You'll be shown a 12-word Secret Recovery Phrase. Write this down securely offline and never share it with anyone.
5. Confirm your Secret Recovery Phrase by selecting the words in the correct order.
6. Your wallet is now set up!

### 3. Adding Core Testnet to Metamask

1. In your Metamask wallet, click on the network dropdown at the top (it likely says "Ethereum Mainnet").
2. Scroll down and click "Add network".
3. Click "Add a network manually" at the bottom of the page.
4. Fill in the following details:
   - Network Name: `Core Testnet`
   - New RPC URL: `https://rpc.test.btcs.network/`
   - Chain ID: `1115`
   - Currency Symbol: `tCORE`
   - Block Explorer URL: `https://scan.test.btcs.network`
5. Click "Save" to add the network.

### 4. Getting Testnet Tokens

1. Make sure you've selected the "Core Testnet" network in Metamask.
2. Copy your wallet address (you can do this by clicking on your account name in Metamask).
3. Go to the [Core Testnet Faucet](https://scan.test.btcs.network/faucet).
4. Paste your wallet address into the faucet website.
5. Complete any captcha or verification steps if required.
6. Click the "Get tCORE" button to receive testnet tokens.
7. Wait a few moments, and you should see the testnet tokens in your Metamask wallet.

Remember, these are testnet tokens with no real value. They're only for testing and development purposes on the Core testnet.

Now you're all set up with Metamask and connected to the Core testnet with some test tokens to use!
 
 ## Setting up the Project

### 1. Fork the Repository

1. Open your web browser and go to <a href="https://github.com/coredao-org/Build-On-Core.git" target="_blank" rel="noopener noreferrer">https://github.com/coredao-org/Build-On-Core.git</a>
2. In the top-right corner of the page, click the "Fork" button.
3. If prompted, select where you want to create the fork (your personal account or an organization).
4. Wait for the forking process to complete. You'll be redirected to your forked repository.

### 2. Clone the Forked Repository

1. Open a terminal on your local machine.
2. Create a new directory for the project and navigate into it:
   ```
   mkdir core-project
   cd core-project
   ```
3. Clone your forked repository (replace `YOUR-USERNAME` with your GitHub username):
   ```
   git clone https://github.com/YOUR-USERNAME/Build-On-Core.git
   ```
4. Navigate into the cloned repository:
   ```
   cd Build-On-Core
   ```

### 3. Navigate to the Specific Folder

Navigate to the Shobhit University folder within the cloned repository:
```
cd University-Dev-Tours/India/Shobhit-University
```

### 4. Clone the Workshop Repository

While inside the Shobhit University folder, clone the Core Workshop repository:
```
git clone https://github.com/b0ney-1/Core-Workshop-C5.git
```

Now you have both repositories set up on your local machine. The Core Workshop repository is nested within the Build-On-Core repository, specifically in the Shobhit University folder.

Your project structure should look like this:
```
core-project/
└── Build-On-Core/
    └── University-Dev-Tours/
        └── India/
            └── Shobhit-University/
                └── Core-Workshop-C5/
```

You're now ready to start working on the project!

## Configuring the Project

After setting up the project, you need to configure it with your personal information and install the necessary dependencies. Follow these steps:

### 1. Update the Environment File

1. Navigate to the Core-Workshop-C5 folder.

2. Locate the `.env` file in this directory.

3. Open the `.env` file with your preferred text editor.

4. Find the line that starts with `PRIVATE_KEY=`.

5. Replace the existing private key with your own Metamask wallet's private key. To get your private key from Metamask:
   - Open Metamask and click on the three dots next to your account name
   - Select "Account details"
   - Click on "Export Private Key"
   - Enter your password and copy the displayed private key

6. Save and close the `.env` file.

   **IMPORTANT**: Never share your private key with anyone or commit it to a public repository. The `.env` file should be listed in your `.gitignore` file to prevent it from being tracked by git.

### 2. Install Dependencies and Compile Contracts

1. Ensure you're in the Core-Workshop-C5 directory in your terminal.

2. Install the project dependencies by running:
   ```
   npm install
   ```
   This command will install all the necessary packages defined in the `package.json` file.

3. After the installation is complete, compile the smart contracts by running:
   ```
   npx hardhat compile
   ```
   This command will compile all the Solidity contracts in your project.

If both commands execute successfully, you should see confirmation messages in your terminal. The `npm install` command will show a list of installed packages, and `npx hardhat compile` will indicate that the compilation was successful.

You have now successfully configured your project and are ready to move on to the next steps!

## Project Deployment

To deploy your project to the Core testnet, follow these steps:

1. Ensure you're in the Core-Workshop-C5 directory in your terminal.

2. Run the following command to deploy your project:
   ```
   npx hardhat ignition deploy ./ignition/modules/deploy.js --network core_testnet
   ```

3. Wait for the deployment process to complete. This may take a few minutes.

4. Once finished, you should see a confirmation message with the deployed contract address. Make sure to save this address as you'll need it for contract verification.

## Contract Verification

After deploying your contract, it's important to verify it on the Core Explorer. This allows others to view and interact with your contract's code. Here's how to do it:

1. Visit the [Core Testnet Explorer](https://scan.test.btcs.network/).

2. In the search bar at the top, paste the contract address you received during deployment.

3. On the contract's page, look for a "Verify and Publish" or similar option. Click on it.

4. You'll be taken to the contract verification page. Here's what you typically need to provide:
   - Contract Address: This should be pre-filled with your contract's address.
   - Compiler Type: Select Solidity(Single File).
   - Compiler Version: Choose the version as `v0.8.24+commit.e11b9ed9`.
   - Select Open source License as MIT License (MIT) and Hit `continue` button 
   - Optimization : Yes.
   - Enter the Solidity Contract Code: Copy and paste your entire Solidity contract code.

5. If your contract uses constructor arguments, you'll need to provide them in ABI-encoded format.

6. If you're using a flattened contract file (combining all imports into one file), make sure to upload this instead of just the main contract file.

7. Double-check all entered information, then click "Verify and Publish".

8. If successful, you'll see a confirmation message, and your contract's page will now show the verified source code.

If you encounter any issues during verification, double-check that the compiler settings match those in your Hardhat configuration, and ensure you're using the correct contract code version that was deployed.

## Create Pull Request

After completing your project, you need to submit your work by creating a pull request. Follow these steps:

1. Manually navigate back to the root directory of the Build-On-Core repository in your file explorer or terminal.

2. Locate the Core-Workshop-C5 directory within the Shobhit-University folder. Manually find and delete the .git folder inside the Core-Workshop-C5 directory. This step is crucial to avoid submodule issues.

   **Note**: The .git folder might be hidden. You may need to enable "Show hidden files" in your file explorer to see it.

3. Open a terminal in the root directory of the Build-On-Core repository and run the following commands:

   Add all changes to git:
   ```
   git add .
   ```

   Commit your changes:
   ```
   git commit -m "Add Core-Workshop-C5 project"
   ```

   Push your changes to your forked repository:
   ```
   git push origin main
   ```

4. Create a Pull Request:
   - Go to your forked repository on GitHub (https://github.com/YOUR-USERNAME/Build-On-Core)
   - Click on the "Contribute" button
   - Click on "Open pull request"
   - You'll be taken to a page titled "Comparing changes"
   - Ensure the base repository is set to `coredao-org/Build-On-Core` and the base branch is `main`
   - Ensure the head repository is set to your fork (`YOUR-USERNAME/Build-On-Core`) and the compare branch is `main`

5. Fill in the Pull Request details:
   - Give your pull request a meaningful title
   - In the description, provide any necessary details about your project
   - If there are any specific instructions or notes for the reviewers, include them here

6. Click on "Create pull request"

Your project is now submitted for review. The Core DAO team will review your pull request and may provide feedback or request changes. Keep an eye on your GitHub notifications for any updates or comments on your pull request.

Remember to respond promptly to any feedback and make any requested changes to ensure a smooth review process.
