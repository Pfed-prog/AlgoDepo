# AlgoDepo

The aim of the following contract is to deposit Algo and Algorant Smart Assets.

This is the building block for more complex applications on Algorand and its ecosystem.

Submission for https://gitcoin.co/issue/c3protocol/hackalgo/1/100028569
## Installation 

Required instalation of Python3 and NPM.

### Python Environment

```bash
pip install virtualenv
virtualenv venv
source venv/bin/activate
pip install -r requirements.txt
```

One line if virtualenv is installed:

```bash
virtualenv venv && source venv/bin/activate && pip install -r requirements.txt
```

To convert Pyteal to teal contract:
```bash
python3 /contracts/contract.py
```

### NPM

To install packages:
```bash
npm i
```

## Run the Deposit App

First add Mnemonic passphrase to ```.env```.
Next go to the [testnet dispenser](https://dispenser.testnet.aws.algodev.network/) to obtain Algo. Create an asset or obtain one from a faucet and enter its id in ```config.js```.

To illustrate the app run:

```bash
npm start
```

Such that

![](https://imgur.com/a/2rC2aiR)

Illustartion of the working app on AlgoExplorer:

https://testnet.algoexplorer.io/application/85314426


### Contract Args

The contract takes 2 args.

The first arg is the type fo transaction: deposit or asa_deposit.
The second arg is the amount deposited.
### Further Resources

[Pyteal](https://pyteal.readthedocs.io/en/stable/index.html)