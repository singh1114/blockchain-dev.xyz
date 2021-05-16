---
layout: post
title: Third generation blockchain - Discussion on Cardano
date: 2021-05-16T12:19:41.391Z
updated_date: 2021-05-16T12:19:42.339Z
description: Issues with the first and second generation of crypto currencies
  and how cardano is working to solve all these problems.
published: true
image: https://i.ibb.co/ZHnkdrV/Third-Generation-Cryptos.png
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
{% include lazyload.html image_src="https://i.ibb.co/ZHnkdrV/Third-Generation-Cryptos.png" image_alt="Third generation blockchain - Discussion on Cardano" image_title="Third generation blockchain - Discussion on Cardano" %}

When we discussed a little about the [history of the blockchain](https://blockchain-dev.xyz/brief-history-of-blockchain/) and how it all started we never discussed the details of how the system works under the hood, all we wanted to do over there was to know how it all started without going to the details.
 
In this post, we are going to discuss in detail, how everything came into the picture. We will also build a story that will explain to us why we needed to move to a better system and what is being built.

## First generation of cryptocurrency - Bitcoin

So, as we already discussed in the history post, the only issue that Bitcoin was trying to solve was to create a system where users can transfer money without using any central system to govern the transaction.

They created a token that was scarce and tradable. This concept was implemented and over the years a lot of people started using it and started finding it useful.

Although this was a groundbreaking implementation, there were a lot of flaws in it and if you wanted to make some change to how Bitcoin works they had to build a new cryptocurrency. This is not an ideal scenario.

There were other problems as well and we will keep talking about them later in the post.

## Second generation of cryptocurrency - Ethereum

This generation provided the ability to the developers to somehow add stuff on top of Blockchain allowing them to build their own stuff using code. So essentially, now developers can push their own stuff onto the Blockchain and build different apps using it.

These apps essentially were not financial service-related. All these things helped Ethereum to have the biggest developer base.

Unfortunately, both of these generations had a few underlying issues that were holding them back from becoming the main source of money transferring. One of them was scalability.

Crypto due to its architecture( more aligned toward security) allowed a limited number of transactions per second and for it to become the mainstream way of transferring money, it had to handle a lot more transactions than it is currently handling.

## Third generation of cryptocurrency - Cardano

The main issue with crypto is not just powering the developers to build stuff on top of the blockchain itself, it is also to build the blockchain as well.

With third-generation cryptocurrencies, we are trying to solve issues like these.

So the third generation of cryptocurrencies is built using 3 main parameters in mind.

* Scalability

* Interoperability

* Sustainability

We will talk about each of them in detail during the post.

## Solving scalability with Cardano

Scalability for every system can be divided into three main points, more so for the cryptocurrency world.

### TPS

Transactions per second is the main scalability issue that we want to tackle. More the number of transactions per second, more the number of users that will be able to transfer money.

### Network Bandwidth

According to the design of Blockchain systems, since it's a peer-to-peer network it's hard to achieve network bandwidth of Megabytes to Gigabytes for it to scale at a level of what financial services are handling today.

### Data storage

Since all the nodes need to have a copy of each transaction on the Blockchain and we need to probably store the transactions that happened like 10 years as well, we need some scalability mechanism in place over there as well.

#### Solving TPS issue with Ouroboros

For handling the TPS issue Cardano is using a peer-reviewed implementation of [Ouroboros](https://cardano.org/ouroboros/).

How do `Ouroboros` works is a separate post of its own. We only want to discuss how it will help scale the TPS for a given chain.

Ouroboros uses a proof of stack algorithm as compared to proof of work algorithm as used by the older version of cryptocurrencies. So, what it essentially does is that it chooses a leader from all the nodes available for a given slot and allow only that to mine the transaction.

With such a technique, we can have a probable secure network given more 51% of the nodes available for mining are not compromised. Remember 51% attack in Silicon Valley, this is what they were talking about.

{% include lazyload.html image_src="https://i.ibb.co/Fqw4Qsz/51.jpg" image_alt="51 percent attack in Silicon Valley" image_title="51 percent attack in Silicon Valley" %}

One more great thing about Ouroboros is that it can run epochs in parrallel and can achieve more TPS when more nodes want to connect.

{% include lazyload.html image_src="https://i.ibb.co/NprFhfr/Screenshot-2021-05-16-at-6-01-17-PM.png" image_alt="Ouroboros Design" image_title="Ouroboros Design" %}

#### Allowing more data to pass - Solving Networking bottlenecks

To solve this, Cardano is trying to make use of a protocol called, [RINA or Recursive InterNetwork Architecture](https://www.martingeddes.com/think-tank/network-architecture-research-tcp-ip-vs-rina/). With the use of this, Cardano will be able to scale at a level of capturing 100s or 1000s of transactions per second.

#### Solving the issue with Data size

Blockchain is architected in a way that all nodes in the chain need to have information related to each and every transaction. But all of this transaction information is not really useful for everyone.

So different concepts can be used with some engineering intelligence to come up with the solution to these.

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

## Solving sustainability - Cardano

With sustainability, we are talking about the continuous development of the chain technology after the initial development is completed.

The main idea behind the proposal is that the big corporations should not take over the development and start building stuff that is important to them and start moving the chain in the direction that they want it to take.

ICOs can be a good way of doing this but they don't offer a reliable flow of money, it is a single-time injection of huge bucks which is generally non-repeatable.
 
To solve this we have to develop a democratic system that is used to fund all the projects that folks want to develop on top of the chain and any changes the chain needs to have to make it better.

There also needs to be a treasury that will have the funds to allocate to the projects that worthy enough and decided by the democratic process.

Also, we need to incentivize folks who participate in this democratic process.

There are people who are trying to figure all these problems and working to implement them.

I believe that once we start to solve some of these problems, we will see old financial institutions start realizing the importance of the Blockchain and start accommodating it to their system.