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

According to the design of Blockchain systems, since it's a peer-to-peer network it's hard to achieve network bandwidth of Megabytes to Gigabytes of Bandwidth.

### Data storage

Since all the nodes need to have a copy of each transaction on the Blockchain and we need to probably store the transactions that happened like 10 years as well, we need some scalability mechanism in place over there as well.

#### Solving TPS issue with Ouroboros

For handling the TPS issue Cardano is using a peer-reviewed implementation of [Ouroboros](https://cardano.org/ouroboros/).  How do `Ouroboros` works is a separate post of its own. We only want to discuss how it will help scale the TPS for a given chain.

{% include lazyload.html image_src="https://i.ibb.co/NprFhfr/Screenshot-2021-05-16-at-6-01-17-PM.png" image_alt="Ouroboros Design" image_title="Ouroboros Design" %}

