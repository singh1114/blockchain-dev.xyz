---
layout: post
title: Building your first Blockchain app - Movie review adding system
date: 2021-05-07T08:42:00.000Z
updated_date: 2021-05-07T08:42:00.000Z
description: Building your first Blockchain app - Movie review adding system using solidity, smart contracts with ethereum
published: true
categories:
  - ethereum
  - bitcoin
  - blockchain
author_name: Ranvir Singh
author_username: ranvir_xyz
series_title: Learning Ethereum Series
series_unique_code: ethereum_dev
series_part: 1
series_page_title: Hash Functions
skip_toc: true
---

To learn about how does the a blockchain works, we will first have to think about how does a website is transferred from the normal internet. Let's say we are trying to build a better IMDb site.

Generally there are 2 entities involved, one is the device from which you are accessing the website, and the other is the system which contain all the data needs to make it possible to make actions on that website.

When you hit enter on an URL all the data is loaded from the server onto your device. All these components which are visible to you are constantly talking to the backend system for almost each and every action that you want to perform. The application might be talking to different servers and server in the background might be talking to a database to store all the information which we might need later.

One thing that we should clearly see is that everything is on central server.

## How does the blockchain works?

Now let's compare how is it different from blockchain and how blockchain application works.

So, in case of blockchain the server side codebase is totally moved onto the blockchain, where ethereum smart contracts help us to build the business logic. The main change about this is that the the main system( blockchain) is distributed and can be accessed by anyone.

So, let's talk about what is blockchain and define it.

## What is a blockchain?

Blockchain is a distributed peer to peer network of nodes connected to one another.

All the nodes makes sure that everything is running smoothely. All of the nodes contain a copy of data and code on the blockchain.

All the records of data and code are bundled together to form a block and they are chained together making a blockchain.

## What all we will need?

We will have to build the business logic which is known as smart contracts and we will need to know a language called `solidity`. All these smart contracts are immutable so once you put them on the blockchain they can't be updated.

Another thing we will need to get started is to ethereum wallet so that we can connect to the blockchain for making these calls to the blockchain.

{% include note.html title="Let's get started" description="Now that we know a little bit about the blockchain and what we are going to develop, let's get started" %}