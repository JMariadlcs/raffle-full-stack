# Raffle Full Stack App

This is a full stack decentralized Raffle App using Chainlink VRF and Chainlink Keepers, Solidity and Next.js from workshop from Chainlink Hackathon Spring 2022.

## Objetives

<< Writing the contracts >>
1. Decentralized RANDOM Raffle.
2. User enter (for a fee).
3. Pick a RANDOM winner.
    1. Autonomous: We never have to interact.
    2. Provable random.

<< Build the Front End >>
1. Buttons using NextJS
2. Deploy it in a decentralized context

## Requirements for creating similar projects from scratch
- Start hardhat project:
```bash
# vscode
.vscode

# hardhat
artifacts
cache
deployments
node_modules
coverage
coverage.json
typechain

# don't push the environment vars!
.env

# Built application files
.DS*
*.apk
*.ap_
*.aab

# Files for the ART/Dalvik VM
*.dex

# Java class files
*.class

# Generated files
bin/
gen/
out/
#  Uncomment the following line in case you need and you don't have the release build type files in your app
# release/

# Gradle files
.gradle/
build/

# Local configuration file (sdk path, etc)
local.properties

# Proguard folder generated by Eclipse
proguard/

# Log Files
*.log

# Android Studio Navigation editor temp files
.navigation/

# Android Studio captures folder
captures/

# IntelliJ
*.iml
.idea/workspace.xml
.idea/tasks.xml
.idea/gradle.xml
.idea/assetWizardSettings.xml
.idea/dictionaries
.idea/libraries
# Android Studio 3 in .gitignore file.
.idea/caches
.idea/modules.xml
# Comment next line if keeping position of elements in Navigation Editor is relevant for you
.idea/navEditor.xml

# Keystore files
# Uncomment the following lines if you do not want to check your keystore files in.
#*.jks
#*.keystore

# External native build folder generated in Android Studio 2.2 and later
.externalNativeBuild

# Google Services (e.g. APIs or Firebase)
# google-services.json

# Freeline
freeline.py
freeline/
freeline_project_description.json

# fastlane
fastlane/report.xml
fastlane/Preview.html
fastlane/screenshots
fastlane/test_output
fastlane/readme.md

# Version control
vcs.xml

# lint
lint/intermediates/
lint/generated/
lint/outputs/
lint/tmp/
# lint/reports/

gas-report.txt
```

- Install dependencies:
```bash
yarn add --dev @nomiclabs/hardhat-ethers@npm:hardhat-deploy-ethers ethers @nomiclabs/hardhat-etherscan @nomiclabs/hardhat-waffle chai ethereum-waffle hardhat hardhat-contract-sizer hardhat-deploy hardhat-gas-reporter prettier prettier-plugin-solidity solhint solidity-coverage dotenv @chainlink/contracts
```
or
```bash
npm install --save-dev @nomiclabs/hardhat-ethers@npm:hardhat-deploy-ethers ethers
npm install @nomiclabs/hardhat-ethers
npm install @chainlink/contracts
npm install dotenv --save
```

## How to compile
```bash
yarn hardhat compile
```
or
```bash
npx hardhat compile
```

## How to deploy

- DISCLAIMER: Always deploy first LOCALLY

- Deploy on Rinkeby:
```bash
yarn hardhat deploy --network rinkeby
```
or
```bash
npx hardhat deploy --network rinkeby
```

## Resources 
- [Hardhat Smart Contract Lottery](https://github.com/PatrickAlphaC/hardhat-smartcontract-lottery-fcc): Patrick's repo that we are building.
- [Front-end Smart Contract Lottery](https://github.com/smartcontractkit/full-blockchain-solidity-course-js#lesson-10-nextjs-smart-contract-lottery-full-stack--front-end): Patrick's repo for the Front-end part.
- [Chainlink Keepers](https://docs.chain.link/docs/chainlink-keepers/introduction/): Used to pick winner AUTOMATICALLY.
- [Chainlink VRF](https://docs.chain.link/docs/get-a-random-number/): Used to pick a winner RANDOMLY.
- [Chainlink VRF addresses](https://docs.chain.link/docs/vrf-contracts/): Used to pick VRF address to deploy contract.
- [Chainlink VRF subscription](https://vrf.chain.link): Used to create a VRF Chainlink subscription id.