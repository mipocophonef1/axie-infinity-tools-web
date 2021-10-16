# Tools for Axie Infinity and Ronin Network (web)
The purpose of this website is to make all the activities related to manage axie infinity scholars much easier. Right now, it is capable of:

- Claim SLP
- Send payouts


# How we do it
We generate the transactions for the blockchain and we give you 2 ways to sign them:


### **Trezor**
If your account is already in trezor, we open the official trezor bridge for you so you can sign the transactions by yourself using your physical device without exposing your seeds and private keys. Also you can set the private key to make the process much faster.


### **Private key**
We might require the secret keys of your accounts to sign the transactions and send them to the blockchain automatically. 
This software is safe to use, you can check your network traffic if you don't trust us. You can ask the community about it too!


# Maintenance fee
We put a lot of effort into creating this, fees and donations allow us to keep working on it!

### **Claim SLP**
No fees for now!

### **Send payouts**
There is a 5 SLP fee per scholar in the code that we take from the manager, scholars receive 100% of their cut. 
Also there is a 100 SLP fee per scholar if necessary (only applied for aromaz scholarships, you'll see a big disclaimer if that's the case).

# How to use it locally

### **Installation**
- Install [Node.js](https://nodejs.org/) (We recommend the LTS version).
- Download the source code.
- Open the terminal (PowerShell on Windows 10), go to the new folder and run `node app.js` to turn on the local server.
- Open a browser and go to `http://localhost:3000`.

### **Set manager address**
- In the text field you must enter a valid ronin address.

Example:

```
ronin:0aa5f40bc4aefcedf3f0baf40fd97bc95049714e
```

### **Add Scholars**
- Click on "Add more scholars" and paste a CSV with this format `address, name, managerPercentage, scholarPaymentAddress, inTrezor, trezorAccountNumber`. Only paste values in the given order without CSV headers. We suggest to store this file locally because each time you reload the website, you'll need to add it again.

    - address: ronin wallet address (ronin:0aa5f40bc4aefcedf3f0baf40fd97bc95049714e)
    - name: whatever you use to identify your scholars (#1 | Scholar 1)
    - managerPercentage: a number from 0 to 100. example 50 (50%)
    - scholarPaymentAddress: personal scholar's ronin address (ronin:0aa5f40bc4aefcedf3f0baf40fd97bc95049714a)
    - inTrezor: true or false depending if the wallet is in trezor or not
    - trezorAccountNumber: 0 for non-trezor accounts and from 1 to 50 for trezor accounts (this is very important, trezor's official bridge asks for this value)

Example:

```
ronin:0aa5f40bc4aefcedf3f0baf40fd97bc95049714e, #1 | Scholar 1, 50, ronin:0aa5f40bc4aefcedf3f0baf40fd97bc95049714a, false, 0
ronin:0aa5f40bc4aefcedf3f0baf40fd97bc95049714f, #2 | Scholar 2, 50, ronin:0aa5f40bc4aefcedf3f0baf40fd97bc95049714a, true, 3
```

### **Add Private keys** (if necessary)

- Click on "Set private keys" to add the private keys if you want to run all the process automatically. Remember you are going to need to add these keys each time you reload the website, we do not store anything. Please, keep this file safe, even if you use trezor if someone gets your recovery seed or private keys, he would be able to create and sign transactions without trezor's physical device.

Example:

```
ronin:0aa5f40bc4aefcedf3f0baf40fd97bc95049714e, 0x33f639697c2d49e840d2d4b7f5ee8e3b82b49eb49f8e3b8e5e3ced6d7386064be
ronin:0aa5f40bc4aefcedf3f0baf40fd97bc95049714f, 0x845e439697c2d5fe5b2d4b7f9ef8e3a77749e840d53db154be5e3ced6d7386063
```

(and no, those aren't the real private keys for those wallets, don't waste your time xD)


# How to get a private key using the oficial Ronin Wallet extension
- Open ronin wallet extension - Go to "Accounts" (top right corner icon) -> Click on "Manage" -> Click on an account -> Press "View private key"


# Warnings
- This software may require  the secret keys the accounts so keep them safe and never share them.
- This software is safe to use. Anyway, you should check it, it wouldn't take more than 30 minutes.
- There is a 5 SLP fee per scholar in the code that you can change. 


# Roadmap
- Improve UI
- Morph eggs (?)
- Breed axies automatically (?)
- Track breeding trees (?)


# Donations

    ronin:0aa5f40bc4aefcedf3f0baf40fd97bc95049714e
    

# Contact
Discord: https://discord.gg/BHkz3Mqqwc

# v0.0.1
![Alt text](src/assets/example--v-0-1-1.png?raw=true "UI")
