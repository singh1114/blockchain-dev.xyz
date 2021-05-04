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
series_title: Learning Ethereum Series
series_unique_code: ethereum_dev
series_part: 1
series_page_title: Hash Functions
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
import hashlib

def get_modulo_coded_output(secret):
    m = hashlib.sha256()
    m.update(secret)
    sha_hash = m.hexdigest()

    output = hash(sha_hash)
    return output % 10
```

This function will always return some fixed value of modulo 10.

```python
>>> get_modulo_coded_output("blockchain-dev.xyz")
10
```

To extend this we can add as many hash functions as possible but we will have a regualar value again, having all those features.

```python
import hashlib

def get_modulo_coded_output(secret1, secret2, secret3):
    m = hashlib.sha256()
    m.update(secret1)
    sha_hash_1 = m.hexdigest()
    m.update(secret2)
    sha_hash_2 = m.hexdigest()
    m.update(secret3)
    sha_hash_3 = m.hexdigest()

    output = hash(sha_hash_1) + hash(sha_hash_2) + hash(sha_hash_3)
    return output % 10
```

```python
>>> get_modulo_coded_output("blockchain-dev.xyz", "blockchain-dev.xyz", "blockchain-dev.xyz")
2
```

This will always return the same result and even a small change in any of the secret will lead to big change the output hash.