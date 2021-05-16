---
layout: post
title: Third generation blockchain - Discussion on Cardano
date: 2021-05-16T12:19:41.391Z
updated_date: 2021-05-16T12:19:42.339Z
published: true
tags:
  - cardano
  - bitcoin
  - ethereum
categories:
  - cardano
  - bitcoin
  - ethereum
author_name: Ranvir Singh
author_username: ranvir_xyz
show_ads: true
show_telegram_signup: false
---
When we discussed a little about the [history of the blockchain](https://blockchain-dev.xyz/brief-history-of-blockchain/) and how it all started we never discussed the details of how the system works under the hood, we just wanted to get started.

In this post, we are going to discuss in detail, how everything came into the picture. We will also build a story that will explain to us why we needed to move to a better system that we already had and what is being built.

## First generation of cryptocurrency - Bitcoin

So, as we already discussed in the history post, the only issue that Bitcoin was trying to solve was to create a system where users can transfer money without using any central system to govern the transaction.

They created a token that was scarce and tradable. This concept was implemented and over the years a lot of people started using it and started finding it useful.

Although this was a groundbreaking implementation, there were a lot of flaws in it. If you wanted to make some change to how Bitcoin works they had to build a new cryptocurrency which was not ideal as well.

There were other problems as well and we will keep talking about them later in the post.

## Second generation of cryptocurrency - Ethereum

This generation provided the ability for the developers to somehow add stuff on top of Blockchain allowing them to build their own stuff using code. So essentially, now developers can push their own stuff onto the Blockchain and build different apps on it.

These apps essentially were not financial service-related. All these things helped Ethereum to have the biggest developer base.

Unfortunately, both of these generations had an issue that was holding them back from becoming the main source of money transferring. Which was scalability.

Crypto due to its architecture( more aligned toward security) allowed a limited number of transactions per second and it to become the mainstream way of transferring money, it had to handle a lot more transactions than it was currently handling.

## Third generation of cryptocurrency - Cardano

The main issue with crypto is just not powering the developers to build stuff on top of the blockchain itself, it is also to build the blockchain itself, as all nodes at a given time, need to have the whole data point with each and every update on it, we need good systems with large storage. With third-generation cryptocurrencies, we are trying to solve issues like this.

So the third generation of cryptocurrencies is built using 3 main parameters in mind.

* Scalability

* Interoperability

* Sustainability

## Solving scalability with Cardano

Scalability for every system can be divided into three main points more so to the cryptocurrency world.

### TPS

Transactions per second are the main scalability point that we want to tackle. More the number of transactions per second, more the number of users that will be able to transfer money.

### Network Bandwidth

According to the design of Blockchain systems, since it's a peer-to-peer network it's hard to achieve network bandwidth of Megabytes to Gigabytes.

### Data storage

Since all the nodes need to have a copy of each transaction on the Blockchain and we need to probably store the transactions that happened like 10 years as well, we need some scalability mechanism in place over there as well.

#### Solving TPS issue with Ouroboros

For handling the TPS issue Cardano is using a peer-reviewed implementation of [Ouroboros](https://cardano.org/ouroboros/). How do `Ouroboros` works is a separate post of its own. We only want to discuss how it will help scale the TPS for a given chain.

Ouroboros uses a proof of stack algorithm as compared to proof of work algorithm as used by older version of cryptocurrencies. So, what it essentially does is that it choses a leader from all the nodes available for a given slot and allow only that to mine the transaction.

With such a technique, we can have a probable secure network given more 51% of the nodes available for mining are not compromised. Remember 51% attack in Silicon Valley, this is what they were talking about.

{% include lazyload.html image_src="https://i.ibb.co/Fqw4Qsz/51.jpg" image_alt="51 percent attack in Silicon Valley" image_title="51 percent attack in Silicon Valley" %}

One more great thing about Ouroboros is that it can run epochs in parrallel and can achieve more TPS when more nodes want to connect.

{% include lazyload.html image_src="https://i.ibb.co/NprFhfr/Screenshot-2021-05-16-at-6-01-17-PM.png" image_alt="Ouroboros Design" image_title="Ouroboros Design" %}

#### Allowing more data to pass - Solving Networking bottlenecks

To solve this, Cardano is trying to make use of a protocol called, [RINA or Recursive InterNetwork Architecture](https://www.martingeddes.com/think-tank/network-architecture-research-tcp-ip-vs-rina/). With the use of this, Cardano will be able to scale at a level of capturing 100s or 1000s of transactions per second.

#### Solving the issue with Data size

Blockchain is architected in a way that all nodes in the chain need to have information related to every transaction. But all of this transaction information is not really useful for everyone. So different concepts can be used with some engineering intelligence to come up with the solution to these.

Some techniques which are useful to control the data size are:

* Pruning

* Subscription

* Compression

* Partitioning

* Subchaining

## Solving interoperability with Cardano

In the open market world of finance which involves banks and other financial institutes, a lot of important things which makes the basis of the whole system are not present in the Blockchain which makes them hard to trust anything done on the Blockchain.

Till the Blockchain environment becomes the sole provider for sharing money over the internet, we have to keep working with these old financial institutes.

Cardano team is working on a solution so that it can help fill this gap between the transaction done in the Blockchain and the transaction done on the Banks website.

For this to work, Cardano needs to cover 3 main areas.

### Metadata

This is the main information of the transaction which tells us why this transaction was done. If the transaction was done on education, it is considered as a good one but if the transaction was done to buy the lottery, it is considered as a bad one( Unless you win one).

### Attribution

Attributing the two parties between whom the transaction was done. It is important for the financial institute/ treasury department to know that this transaction was not done to finance terror activity or something fishy.

### Compliance

This is something on the same lines of attribution. This helps us realize that the given transaction is a valid one. It is done to make sure that your company is not working for terror financing or using it to fund malicious activities.

### Knowing across Blockchain transactions

The system also needs to know about the transactions happening on the other blockchain so that they can validate a transaction on the other chain as well. So that there is no single crypto to rule them all.

{% include note.html title="All of this is optional and not visible to everyone" description="One thing that we need to understand is that all of these are optional and also these data points are only visible to one entity or sometimes both of the parties involved and would be put on the blockchain using some hashing mechanism." %}