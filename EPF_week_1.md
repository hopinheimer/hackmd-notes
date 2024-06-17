
# Manas (hopinheimer) - Week 1

A week of exploration on PeerDAS, I stumble upon a lot of new topics to explore and here is an update circling them. 

## Research Rationale

Upon close observation of Data Availablity and PeerDAS, I discovered that the protocol has a fair deal of upgrades underway based on various different rationale by various different people. I tried to approach my research in a sort of **heuristic Breadth First Search** scheme which eventually lead to a general area along **data** and **networking** as it becomes evident further in this update. I tried to understand the fundamental idea of the protocol's design and the tenets used to fabricate that. My experience of writing epf wiki on [*design rationale*](https://epf.wiki/#/wiki/protocol/design-rationale) also aided the approach.

Then came the poking around part. Ethereum is a labyrinthian piece of code and is 
comprised of seemingly [composable](https://en.wikipedia.org/wiki/Composability) components. I tried to run as many projects locally as possible where projects like kurtosis were of great help.

![meme](https://hackmd.io/_uploads/SkDDx22BR.png)

## Projects running locally

These are the projects that kept my laptop plugged in the entire week.

- [trin](https://github.com/ethereum/trin) portal client 
- [mev boost relay](https://github.com/flashbots/mev-boost-relay) ~*flashbots* 
- [kurtosis](https://github.com/ethpandaops/ethereum-package) geth - lighthouse
- [reth](https://github.com/paradigmxyz/reth) ~paradigm
- [hive](https://github.com/ethereum/hive) (still working on it)


there are a few more projects I'd like to run a local setup of over the next week.

## Research

This week I attended the ACD meeting and the peerDAS and ePBS breakrooms to have a brief context about the current state and research being conducted on the protocol, based on which I tried to dig into some of the formative previous changes. To my understanding changes can be categorized into ***optimization changes*** and ***feature changes*** (while some might say features **are** optimization changes, I'll change the statement to a better one later :grin:). I tried to focus mostly on some of the feature changes this week. 

TL;DR:

- **EIP-1559**: [Fee market change for ETH 1.0 chain](https://eips.ethereum.org/EIPS/eip-1559)
- **EIP-2718**: [Typed Transaction Envelope](https://eips.ethereum.org/EIPS/eip-2718)
- **ePBS**: [enshrined Proposer Builder Separation](https://ethresear.ch/t/why-enshrine-proposer-builder-separation-a-viable-path-to-epbs/15710)
- **proto-danksharding**: [Shard blob transaction](https://eips.ethereum.org/EIPS/eip-4844)
- **Portal Network**: [p2p federated data provider network](https://www.ethportal.net/overview)
- **Inclusion lists**: [spec](https://ethresear.ch/t/specing-out-forward-inclusion-list-w-dedicated-gas-limits/17115)
- **EOF**: [extensible and versioned container format for the EVM with a once-off validation at deploy time](https://eips.ethereum.org/EIPS/eip-3540)
- **SSZ**: [simple serialize](https://ethresear.ch/t/replacing-ssz-with-rlp-zip-and-sha256/5706)
- **Verkle**: [spec](https://ethereum.org/en/roadmap/verkle-trees/)

> :bulb: I will be adding rationale behind each one of these that I learnt.

I found myself interested in [Portal Network](https://github.com/ethereum/portal-network-specs), since I originally tried to implement along similar lines back when I was in school based on [uTP](https://www.bittorrent.org/beps/bep_0029.html) by bitorrent.  I still haven't finalized on what to work on but portal network or peerDAS are good candidates for this week

## Final Thoughts

I have a few tasks complete the following week 
1. golang implementation of a PoC for portal network spec 
2. PeerDAS grandine implementation opportunity
3. libp2p study

## Literature


1. Inclusion lists <> PBS
    1. https://notes.ethereum.org/@vbuterin/pbs_censorship_resistance
    2. https://ethereum-magicians.org/t/eip-7547-inclusion-lists/17474
    3. https://eips.ethereum.org/EIPS/eip-7547
    4. https://gist.github.com/michaelneuder/dfe5699cb245bc99fbc718031c773008
    5. https://notes.ethereum.org/@vbuterin/pbs_censorship_resistance

1. EVM Object format (EOF)
    1. https://ethereum-magicians.org/t/evm-object-format-eof/5727
    2. https://notes.ethereum.org/@axic/evm-object-format



