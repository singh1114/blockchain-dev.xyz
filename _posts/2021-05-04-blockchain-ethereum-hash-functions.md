---
layout: post
title: Hash Functions - What are hash functions in a Blockchain?
date: 2021-05-04T08:42:00.000Z
updated_date: 2021-05-04T08:42:00.000Z
description: What are hash functions in a Blockchain?
published: true
categories:
  - ethereum
  - bitcoin
  - blockchain
author_name: Ranvir Singh
author_username: ranvir_xyz
series_title: Learning Ethereum Post
series_unique_code: ethereum_dev
series_part: 1
series_page_title: Hash Functions - What are hash functions in a Blockchain?
skip_toc: true
---

Hash Functions - What are hash functions in a Blockchain?

Hi there, welcome back. Today we are going to discuss few things realted to hash and discuss how it works.

There are a few features according to which you can define a hash,

* The result is determinstic.
* It's really hard to guess the key( Generally).
* The size of output is same.
* You can pass anything as the input to this particular hash function.
* Its one directional, you can't guess the secret if you know the hash.


A fairly simple way to describe this would be to see the example of `sha256` with modulo 10 returned.

```python
def get_color_coded_output(secret):
    hash = sha256(secret)

    output = hash.getKeyHash()
    return output % 10
```

This function will always return some fixed value of modulo 10.

To extend this we can add as many hash functions as possible but we will have a regualar value again, having all those features.

```python
def get_color_coded_output(secret1, secret2, secret3):
    hash = sha256(secret1)
    hash2 = sha256(secret2)
    hash3 = sha256(secret3)


    output = hash.getKeyHash() + hash2.getKeyHash() + hash3.getKeyHash()
    return output % 10
```