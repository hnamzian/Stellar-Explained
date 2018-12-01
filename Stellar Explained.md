# Stellar Explained

- references:

  - <https://www.stellar.org/how-it-works/stellar-basics/#how-it-works>
  - <https://www.stellar.org/how-it-works/stellar-basics/explainers/>
  - <https://www.stellar.org/how-it-works/stellar-basics/#>
  - <https://www.stellar.org/how-it-works/use-cases/>

## Overview

- Stellar is a platform that connects **banks**, **payments systems**, and **people**.

- Integrate to move money **quickly**, **reliably**, and at almost **no cost**.

![logo](images/stellar.png "logo")

## How Stellar Network operates

- Q: How to send EUR to your friend using USD on the Stellar Network?

- A **decentralised network** of servers power the **distributed ledger**
- The ledger records every **transaction** in the system
- A copy of the global ledger exists on each Stellar server

![Stellar Network](images/stellar-network.png "Stellar Network")

- Every **2-5 seconds** servers communicate with each other to **verify transactions** and **sync the ledger** (**consensus process**)

![Stellar Consensus](./images/Stellar-consensus.png "Stellar Consensus")

- **Anchors** are provided as bridges between given currencies and Stellar network
- The ledger records your money as **Credit**, which is issued by anchors

![Credit table](images/credit-table.png "credit table")

- Anchors have to be trusted to hold your money and honor your withdrawals
- Issued credits can be sent and received on the network

![Stellar exchange](images/Stellar-exchange.png "Stellar exchange")

- Thanks to **distributed exchange**, you can send EUR credits with your USD credit balance
- Your friend receive EUR credit which can withdraw using an anchor supporting EUR

![process overview](images/process-overview.png "process overview")

## Anchor, trust and credit

![gateway](images/gateway.png "gateway")

- Entities that people trust to **hold their deposits** and **issue credits** into the Stellar network for those deposits.

- They act as a bridge between different currencies and the Stellar network.

- All money transactions in the Stellar network (except the native digital currency of lumens) occur in the form of credit issued by anchors.

### What does Anchors do

    1- They take your deposit and issue the corresponding credit to your account address on the Stellar ledger.

    2- You can make a withdrawal by bringing them credit they issued.

### Anchors vs PayPal

To use PayPal you deposit money in from your bank account. You recieve credit in your PayPal account. You can send your credit to anyone else trusting to PayPal, and then convert it to real money using PayPal by withdrawing it to the bank.

Anchors perform the same function in Stellar. The difference is, all the "Paypals" and other anchors are operating on the same network so they can all transact with each other now. People can now easily send and exchange all these different anchor credits with each other.

## Distributed Exchange

![distributed exchange](images/distributed-exchange.png "distributed exchange")

Stellar ledger can be thought of global marketplace for offers of buy/sell currencies committed by people to exchange one type of currency to another one.

All these offers form what is called an orderbook. There is an orderbook for each currency/issuer pair. So if you are wanting to exchange Virgin Bank/EUR for bitstamp/BTC you look at that particular order book in the ledger to see what people are buying and selling it for.

This allows people to not only buy and sell currencies in a foreign exchange like manner but also to convert currencies seamlessly during transactions.

## Multi-currency transactions

![multi currency](images/multicurrency.png "multi currency")

Stellar allows you to send any currency you hold to anyone else in a different currency through the built-in distributed exchange. People can receive any currency through an anchor they added.

### possible ways the transaction can happen

- Conversion through an offer

Stellar finds an offer on the internal USD/EUR exchange for someone wanting to buy EUR for USD and automatically makes the exchange between the two parties.

- Using lumens as an intermediary currency

Stellar looks for offers on the network asking for USD in exchange for lumens (the native — purely digital — currency). It simultaneously looks for an offer asking for lumens in exchange for euros. The network makes those exchanges and sends Bob the resulting euro credit.

- Chain of conversions

If there are no explicit relationship between offers to buy and sell, Stellar tries to find offers from the network that will lead a chain of conversions from EUR to USD. For example, EUR to AUD, AUD to BTC, BTC to XLM, XLM to USD.