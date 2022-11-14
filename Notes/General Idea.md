# Annonymous by design scientific papers uploading protocol using ZKs and decentralized technologies

---
## Upload Workflow

1. We generate a *private-key* + *user* completely **offchain**.
2. The user can upload a file.
	1. This file goes to [[IPFS]].
	2. We retrieve the file's *IPFS* hash.
3. Onchain there is a [TCR](https://medium.com/@tokencuratedregistry/the-token-curated-registry-whitepaper-bd2fb29299d6) ([[Token Curated Registry]]) + contract containing file metadata such as tags, *IPFS* link ... + The puzzle that can only be solved by the owner of the private key related to the user that uploaded the paper.
	1. Once uploaded [The graph](https://thegraph.com/en/) will take care of indexing in order to filter by certain criteria in the front-end.

---

## Review Workflow

1. The review process starts once the paper has been uploaded and indexed.
2. The review process never ends -> This leads to a *free market* kind of karma ranking where the best works will be at the top, and new ones or bad ones, at the bottom
3. At any moment in the review process, you can decide wether or not, you want to claim the ownership of your work. You can basically choose wether you want to be public since the beginning (maybe by adding your name on the paper), remain annonymous forever, or perhaps you want to be annonnymous for just some amount of time ***You decide***

---

## Tools Used

- ZK library: [[Circom]] -> The most used library and the one with more documentation and example code available. *Tornado cash* was built using this tool.