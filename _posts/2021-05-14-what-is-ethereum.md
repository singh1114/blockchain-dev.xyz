---
layout: post
title: What is Ethereum and how to work with it
date: 2021-05-14T16:45:25.734Z
updated_date: 2021-05-14T16:45:25.785Z
description: What is Ethereum and how to work with it
published: true
tags:
  - blockchain
  - ethereum
categories:
  - blockchain
  - ethereum
author_name: Ranvir Singh
author_username: ranvir_xyz
show_ads: true
show_telegram_signup: false
series_unique_code: ethereum-and-solidity-the-complete-developers-guide
series_part: "2"
series_page_title: What is Ethereum
series_title: Ethereum and solidity complete developer guide
previous_slug: brief-history-of-blockchain
skip_from_listing: false
---
Ethereum at its heart is just a network of computers( nodes) talking to each other and having the same data as other nodes are having which can be used to power a ton of different stuff. Transferring money is just one of its use cases.

{% include lazyload.html image_src="https://i.ibb.co/rc2Pd1J/Screenshot-2021-05-15-at-12-27-54-AM.png" image_alt="Ethereum node connection" image_title="Ethereum node connection" %}

There are a ton of Ethereum networks out there. Of course, there is the main one where all the action happens. This main network is the one everyone deploys their production apps to and also this is the on which Ethereum coin is traded.

There are other networks based on the Ethereum blockchain system as well. Some are just for testing stuff, some are for other purposes as well. You can also launch your private Ethereum network. We of course in this list of posts will be creating a local network for testing our stuff.

These networks are made using the connection of nodes. Each of these nodes needs to have the Ethereum client installed on them to be part of the network. Anyone with this client installed can run the node. Each of the nodes will have a copy of the data on the network.

Each movement of the data is stored as a separate entry in each of the nodes separately. This makes the blockchain no different from a database with one difference that you cannot delete or update the old data.

But if you have read details about log-based databases like `Cassandra storage engine`, this is what they do internally, but they provide some other mechanisms to allow updates and deletes.

This is more like a `Kafka-based` approach.

If you are a software engineer already, it helps to make those connections with the existing systems. It helps you to understand stuff better.

Now that we have understood the basics of what Ethereum is, let's talk about the ways in which we can work with it both as a developer and as a consumer.

As a developer, we might want to connect to the network to run our apps on the network using code. There are a ton of ways of doing that. `web3.js` is one that we are going to use. We are also going to use `Solidity` to create smart contracts.

On the other hand, as a consumer, we can use an extension like metamask to connect to the network and run Ethereum based applications in our browser. Brave browser is the browser that is working to bring in-browser support to decentralized apps.

We are going to deep dive into each of them separately in our upcoming posts.

Till then! Enjoy 🎉