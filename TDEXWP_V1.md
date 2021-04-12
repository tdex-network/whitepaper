# TDEX: A Decentralised Vision to Leverage Atomic Swaps for Liquid Finance (LiFi)

**TDEX white paper | Version 1.0 | October 2020**

**Abstract:** T(True)DEX is the first-of-its-kind, atomic-swap based, privacy-prioritised Decentralised Exchange (DEX) platform built on the Liquid Network. As a community-oriented, open-source solution, it aims to become the framework for a fast and secure cyberspace for crypto-users, as well as a secondary market for Liquid Assets. In doing so, TDEX facilitates liquidity generation in a way that leverages Bitcoin&#39;s security but substantially mitigates its privacy and fungibility shortcomings, thus strengthening the foundation for Liquid Finance (LiFi)—the Liquid Network&#39;s version of Decentralised Finance (DeFi). In this white paper, we elaborate on the project&#39;s ecosystem and the underlying vision that shines as a guiding light.

## 1. Introduction

Technological innovations are pivotal to human progress, and more often than not, they save and make lives better. Considering its immense significance, technology should ideally be accessible to all, equally and adequately. Yet, that hasn&#39;t been the case.

Focusing on the finance sector, one cannot deny that innovations in FinTech have substantially enhanced the overall end-user experience: one-touch payments, digital passbooks, e-KYC, and so on. However, although the acquired ease-of-use supposedly drives wider usage, in reality, traditional financial systems have been structurally exclusive of the global unbanked population of around [1.7 billion](https://globalfindex.worldbank.org/chapters/unbanked) adults.

Privacy, on the other hand, has been drastically violated. Governmental institutions and for-profit corporations not only pry into the user&#39;s online activities, but also misuse their personal data to monitor, censor, and advertise. Arguably, this amounts to an infringement of a very basic right of the user.

Primarily, this is a direct outcome of the involvement of multiple intermediaries like banks, governments, agents, brokers, and so on. These intermediaries serve as the overseers or &quot;trust&quot;, and in the process, emerge as central points of control.

### 1.1 Bitcoin: Combining User-Oriented Technology

In 2008, Satoshi Nakamoto released the Bitcoin [white paper](https://nakamotoinstitute.org/bitcoin/), presenting a combination of four potent, _user-oriented_ technologies—blockchain, cryptography, proof-of-work, and peer-to-peer—in the sense that they reinstate control with users, rather than with centralised governing entities. The innovation facilitated a new economic paradigm for secure, peer-to-peer monetary transactions within a distributed and fully-decentralised ecosystem. By tackling the problem of double-spending without using the trust-based model, Satoshi effectively eliminated third-party intermediaries from the process and replaced them with a computerised algorithm.

Nevertheless, despite having all the features of sound money and store of value, Bitcoin, in its skeletal form, falls short of its promise of privacy and fungibility. In other words, Bitcoin transactions are pseudonymous and not anonymous, while its fungibility is challenged by chain analysis and so on. Furthermore, to achieve optimal security and resilience, Bitcoin&#39;s core makes essential compromises in scalability, rendering it inefficient for several crypto-based solutions and functionalities. Later in the paper, we discuss how the Liquid sidechain addresses these issues with Bitcoin&#39;s Layer-1.

### 1.2 The Problem of Generating Consistent Value

Over the past decade, the community has become overcrowded and almost saturated with crypto-assets. Backed by disruptive promises, these assets have rapidly become popular. Yet, given the mammoth losses conceded to scams, hacks, and failed projects, one must critically examine whether a majority of these endeavours actually contribute towards the community&#39;s long-term progress. More importantly, how do they fare in terms of the domain&#39;s foundational principles?

**Custodial Exchanges**. For consistency with TDEX&#39;s immediate purpose, let&#39;s take the example of centralised exchanges which are presently the primary gateway for interacting with most crypto-assets. To meet regulatory obligations and ensure liquidity, most exchange platforms are custodial: they retain control over the user&#39;s funds, as well as the private keys of their exchange-hosted wallet.

A majority of custodial exchanges are owned, managed, and governed by singular entities, while funds and data are stored in centralised servers. Consequently, to trade and transact on these exchanges, users must interact with such siloed servers that represent a _single-point-of-failure_, thus exposing them to high risks of security and privacy breaches, censorship, as well as fund loss.

**Decentralised Exchanges**. As an alternative to custodial exchanges, several decentralised exchanges have proliferated. In general, they implement algorithmic market making protocols, commonly known as _Automated Market Makers_ or AMMs, determining prices through demand-supply metrics, without third-party interference. However, they come with their own set of perils, of which, scalability concerns are the most relevant in the context of this paper.

Partially because of their underlying blockchains and also as a downside of implementing smart contracts, a majority of DEXs are non-scalable, thus resulting in very high transaction fees in periods of network congestion. In their present form, as a DEX becomes more popular, it also becomes infinitely costlier. Furthermore, bugs in smart contracts have emerged as a common peril for the industry, leading to users suffering substantial losses from hacks and breaches.

### 1.3 The TDEX Project

Developed by SevenLabs, TDEX is a community-oriented, Elements-based decentralised exchange built on the Liquid Network. Leveraging the combined security, usability, and speed of the Bitcoin-Liquid framework, TDEX envisions a fast, secure, and truly-decentralised trading experience in Liquid Assets (L-Assets).

The underlying TSWAP protocol implements atomic swaps and solves the liquidity problem through several &quot;zero-to-one&quot; incentives. TDEX also empowers liquidity providers by enabling them to choose their market-making strategy. On the other hand, traders gain from competitive rates, faster settlements, lower slippage, and better security.

In the following sections, we discuss the background and foreground elements of the TDEX platform. In the process, we highlight how the platform could emerge as a backbone network for Liquid Finance (LiFi), enabling professional traders and business owners to manage, transact, and invest within a privacy-prioritised environment.

## 2. The Framework: Security, Privacy, and Speed

Leveraging an Elements-based core, TDEX is deployed on the Liquid Network. As a Bitcoin sidechain, Liquid inherits and enhances its security, while improving the privacy, fungibility, and scalability aspects. In this segment, we elucidate the rationale for adopting liquid as the framework for TDEX.

To effectively resolve the aforementioned crises of decentralised trading, TDEX envisions a holistic, two-fold solution. On one hand, it must resolve some of the community&#39;s primitive concerns, such as latency, inadequate privacy, and the threats to fungibility. On the other hand, it must widen the horizon of open financial solutions, enabling newer functionalities as compared to Bitcoin&#39;s core. In other words, TDEX intends to diversify the purpose of Bitcoin&#39;s layer-1 and it is precisely on this point that its vision collates with that of Liquid, a layer-2 bitcoin sidechain.

As the authors of the Liquid [white paper](https://blockstream.com/assets/downloads/pdf/liquid-whitepaper.pdf) rightly point out, _&quot;for the high-speed world of the cryptocurrency trader, transaction fees, variance in settlement times, publicly-broadcast transactions, as well as the risks of chain reorganizations can incur significant costs during their trading activities.&quot;_

Apart from the network&#39;s Byzantine Fault Tolerant (BFT) consensus that we shall discuss briefly, implementations such as Confidential Transactions and Asset Issuance appeared to be the most relevant for TDEX&#39;s purpose.

### 2.1 The Strong Federation &amp; Liquid&#39;s BFT Consensus

To put it simply, Liquid works with a peg-in-peg-out mechanism, secured by a _globally and culturally distributed_ set of &quot;functionaries&quot;, collectively forming a &quot;[Strong Federation](https://blockstream.com/strong-federations.pdf)&quot; of validators. To ensure that these functionaries have their _skin in the game_, the protocol requires them to be exchanges, brokers, and so on—that is, entities with substantial motivation for ensuring the stability and progress of the Bitcoin network. The federation signs blocks, transactions, and _pegs_ on Liquid using &quot;key modules&quot; which enforce algorithmic logic to restrict unauthorised forks and transactions. Furthermore, the underlying BFT consensus implements a _round-robin, three-phase commit scheme_ and blocks are signed every minute, without involving the risk of chain reorganisation.

As opposed to the _random Poisson distribution_ of Bitcoin&#39;s PoW consensus, Liquid&#39;s federated two-way peg implies manifold improvements in transactional latency. In turn, this would allow almost real-time trade and transaction settlement (~2 minutes) on the TDEX network, while preserving the platform&#39;s decentralisation since the federation is a set of mutually non-trusting participants. Furthermore, Liquid adopts a threshold vector, , where _n_ is the total number of functionaries and _k_ represents the minimum number of signatures required for a block to be considered valid. Notwithstanding the shortcoming that every functionary must have an adequately-synced clock, said vector enables the network to achieve both _safety_ and _liveness_, which ultimately translate to greater security and uptime for TDEX.

### 2.2 Confidential Transactions

In the process of developing TDEX, the realisation that privacy is a fundamental human right presented itself as the substratum for a majority of choices. Bitcoin&#39;s public ledger records every transaction without linking them directly to the sender, and apparently, this is sufficient for privacy. However, a closer look reveals that _pseudonymity_, to a considerable extent, falls short of ensuring _autonomy_ for the user. For instance, _chain analysis_ and tracing the transaction history related to a certain public key could effectively negate the user&#39;s pseudonymity. Moreover, the patterns revealed in the process could also be used to classify _good_ and _bad_ coins, which is a threat to _fungibility_. Presently, solutions are being developed to resolve these issues, which include TDEX&#39;s implementation.

One must note that privacy isn&#39;t merely about _secrecy_—rather, it implies that the user controls _if and when_ to reveal a certain piece of information about themselves. In this regard, Liquid enhances Bitcoin&#39;s privacy metrics, and thus, again, its path intersects with TDEX&#39;s journey.

Implementing components such as _homomorphic commitments_, _Diffie-Hellman key exchange_, and _range proofs_, among others, Liquid enables &quot;[Confidential Transactions](https://blockstream.com/bitcoin17-final41.pdf)&#39;&#39; wherein both the amount and the asset type are blinded. In other words, the amount and type of the asset being transacted is encrypted in a way such that it can neither be decrypted (opened) using another value, nor can it be determined given the commitment. Presuming the _Unspent Transaction Output_ (UTXO) model, this method proves the validity of a transaction by proving that the _ **total input = total output** _, meaning that there has been no inflation, destruction, or double-spending in the process. Furthermore, the network leverages _Asset Surjection Proof_ (ASP)—a form of Zero-Knowledge Proofs wherein, to put it simply, the &#39;_asset tag_&#39; proves that it is committed to a _spent asset_, but doesn&#39;t reveal which one.

As a primary cogwheel in Liquid&#39;s machine, confidential transactions adopt asymmetric encryptions using _blinding keys_—that is, a private-public key pair. Among other outcomes, it minimises the risks of interception during the key exchange process, thus making transactions optimally private and censorship-resistant. In simple terms, the process may be summarised as follows:

- The asset owner (sender), say Marie, broadcasts the public address for her intended transaction (swap). Understandably, this is visible to the entire network.
- An interested receiver, say Alice, _encodes her public blinding key_ into an address which she shares with Marie. In the case of TSWAP, this exchange occurs over an encrypted messaging protocol which, apart from ensuring security, also enables both parties to verify the UTXOs involved in the transaction.
- Upon receiving the message, Marie builds the transaction and encrypts it with Alice&#39;s public address. Alice (the receiver) is the only person with the associated private key for this transaction, and thus, she alone can decrypt the transaction after it is recorded on the blockchain—not even Marie.

Consequently, the network addresses such transactional needs where a blanket &quot;transparency&quot; is rather undesirable. For instance, confidential transactions enable businesses to conduct financial processes in a way that is decentralised and verifiable, but simultaneously protects sensitive information from public exposure. Similarly, the principle strengthens the impetus for crypto adoption in other relevant sectors, such as governmental finance, and so on.

## 3. The TDEX Ecosystem

The emergence of decentralised solutions on the Liquid Network—or, as Adam Back, the CEO of Blockstream, calls it, Liquid Finance or LiFi—has been gaining substantial strength recently. Consequently, an increasing amount of value is being generated on the network, especially in the form of Liquid Assets. In turn, TDEX strives to address the community&#39;s growing demand for a decentralised secondary market for these assets, apart from being an open-source toolkit to foster further innovation.

In the previous sections, we have discussed TDEX&#39;s framework and the reasons behind some of its crucial choices. Now, we elaborate on the platform&#39;s ecosystem, presenting the reader with an overview of the protocols and implementations.

### 3.1 The Technical Pillars: Basics of True DEX (BOTD)

At TDEX&#39;s core, there are four protocols—_Message_, _Transport, Swap_, and _Trade_—which we shall discuss in this segment. However, in this regard, the paper deliberately refrains from elaborating the complete technical expositions which are available in the technical documentations under [TDEX Specifications](https://specs.tdex.network/).

#### 3.1.1 Message Protocol: BOTD #1

A fundamental, so-called primitive requirement for TDEX&#39;s decentralised network is a secure, two-way messaging channel to connect counterparties. Such a connection has to be reliable, stable, peer-to-peer (P2P), and above all, privacy-prioritised. Leveraging Liquid, TDEX can meet these requirements for _confidential communications_. Further, to serialise these messages, TDEX implements Google&#39;s _Protocol Buffers_—a platform and language agnostic method for serialising structured data.

#### 3.1.2 Transport Protocol: BOTD #2

To transact on the network, daemons (users) require P2P transport channels, wherein the need for confidentiality and security applies similarly as the message protocol. In this regard, TDEX provides several options with a varying degree of privacy which the user can implement either in isolation or in combination—_Clear Text_ (insecure), _Onion Service_ (onion), _Server-Side TLS_ (TLS), _Mutual TLS_ (mTLS), and _Noise\_XK\_secp256k1\_ChaChaPoly\_SHA256_ (noise). While participating in the TDEX network, users must declare their implemented transport channel.

#### 3.1.3 Swap Protocol: BOTD #3

The TSWAP protocol is a secure, atomic-swap-based implementation enabling peers on the network to exchange signed messages and transactions. As the means of bridging the **Proposer** and **Responder** , TSWAP is a pivotal element of the TDEX ecosystem. Leveraging aforementioned message and transport protocols, TSWAP primarily has four sub-elements:

- **SwapRequest:**  **t**** he proposer** initiates the swap.
- **SwapAccept:** the responder accepts the request.
- **SwapComplete:** the proposer confirms the secure connection.
- **SwapFail:** either party announces the swap&#39;s termination upon failure. In the future, an additional element—_failure\_code—_could be implemented to denote the reason behind the failure.

#### 3.1.4 Trade Protocol: BOTD #4

Arguably the most crucial implementation for TDEX, the Trade Protocol combines all of the previous BOTDs to define the public interface for the non-custodial exchange. Contrary to the order-book model of custodial exchanges, this protocol allows _traders_ and _market makers_ to connect directly using atomic-swaps.

At a later section, we shall discuss the ecosystem for traders and liquidity providers. Presently, it should suffice to mention that market makers represent _always-on_ daemons and provide proportional liquidity to **Base-Quote** asset pairs. In the future, TDEX would adopt [Simplicity](https://blockstream.com/simplicity.pdf)-based contracts to further enhance the platform&#39;s security and privacy, while also enabling wider functionalities.

### 3.2 TDEX for Market Makers

On the TDEX network, _Market Makers_ are such entities that provide liquidity to asset pairs to be traded on the exchange, and thus, may also be called _Liquidity Providers_ ( **Provider** ). The Provider&#39;s primary function is to hold a mutually-pegged pair of a Quote Asset (quote\_asset) and a Base Asset (base\_asset). It must be noted, however, that this applies to any asset pair and not necessarily the Bitcoin-pegged ones.

As a solution for the classic problem of [_Double Coincidence of Wants_](https://www.oxfordreference.com/view/10.1093/oi/authority.20110803095622703), TDEX enables market markers to run _always-on_ endpoints, while also revealing its publicly reachable address using either of the channels defined in BOTD #2. This ensures readily available markets for the traders, thus addressing one of the major pain-points of decentralised exchanges.

#### 3.2.1 Daemon Implementation

To participate as a Provider, one has to implement a Daemon on the network either by running it through Docker or as a Standalone entity (Read More: [Daemon Implementation Procedure](https://docs.tdex.network/tdex-daemon.html)). A standard daemon on TDEX exposes two HTTP/2 gRPC endpoints—the **Trader Interface** (public) and the **Operator Interface** (private). While the public interface represents the port for traders (default: 9945), the private interface (default: 9000) is used for the market maker&#39;s internal transactions. Further, for optimal security, each daemon has a pre-embedded [Blockstream Green](https://help.blockstream.com/hc/en-us/categories/900000056183-Blockstream-Green) or Liquid Wallet.

#### 3.2.2 Market Making Strategies

One of TDEX&#39;s differentiating elements is that it provides multiple market-making options for Providers, thus significantly widening their scope. In other words, TDEX lets market makers choose or create their strategies, rather than imposing one or the other.

By default, the protocol adopts a _Constant Function Market-Making_ (CFMM) strategy for determining asset prices. However, market makers also have the option to implement _pluggable_ (external) price feeds using a custom API. Considering that business involvement would be pivotal to TDEX&#39;s success, custom market-making strategies are among the platform&#39;s most crucial functionalities, especially because it simultaneously upholds the logic of users&#39; choice. In other words, while Providers have the choice to select their pricing strategy, the platform&#39;s sovereign traders have the capacity to choose or reject these strategies.

#### 3.2.3 Swap Fee

While the _base\_asset-quote\_asset_ reserve ratio shifts with every trade, TDEX ensures consistency in the overall market size by levying a minimal swap fee on every trade and adding it to the reserves. Considering that arbitrage shall motivate a consistent transactional flow, in cases where the market maker implements an AMM-based strategy, the revenue generated from the fee should rise over time.

Parallelly, however, TDEX adopts the [P2EP](https://en.bitcoin.it/wiki/PayJoin)[mechanism](https://en.bitcoin.it/wiki/PayJoin), thus minimising the blockchain space required by transactions which effectively optimises the fee involved. This is done to ensure a fair and level playground for both Traders and Providers on the platform.

#### 3.2.4 Liquidity Pools (Future Implementation)

Further along its intended roadmap, TDEX would implement a _non-custodial_ functionality which that can act as the framework for daemons to connect together and pool their assets. Once achieved, this would ensure greater and more consistent liquidity on the platform, as well as expose a single endpoint for traders&#39; convenience. In turn, TDEX will be able to accommodate financial demands at scale.

As such, the Provider creating a pool will be the _Pool Master_ and other providers will be able to join the _distributed service mesh_ to aggregate liquidity. As an incentive, the pool master will be vested with the capacity to determine the base price for the pool&#39;s assets and traders will have to look up the provider&#39;s aggregated spot prices. For any given asset, a provider can either run alone or join a pool, but they cannot assume both positions simultaneously.

### 3.3 TDEX for Traders

In the context of TDEX, the _market_ is any pair of base and quote assets that can be swapped atomically. As mentioned under BOTD #3, a **Proposer** has to initiate swaps on TDEX, and alternatively, represents a Trader on the network. In other words, a Trader on TDEX is any user that fully implements the Trade Protocol (BOTD #4). In doing so, she connects with the previously-discussed Trader Interface—the public port of the Provider&#39;s daemon—and agrees to trade at the stipulated market rate.

In general, trading on TDEX is similar to any other atomic-swap-based exchange, meaning that the trader can swap equal proportions (by market value) of both assets in the pair. However, unlike a majority of its peers from other networks, TDEX&#39;s framework ensures confidentiality, faster settlements, and minimal or no slippage. Moreover, being non-custodial, TDEX relieves the trader of concerns about losing funds to hacks and breaches.

#### 3.3.1 Software Development Kits: TDEX&#39;s Open-Source Contribution for LiFi

Apart from the default UI, the platform also enables traders to deploy their custom client using TDEX&#39;s software development kits (SDK). In the initial phase, this can be done using [JavaScript](https://docs.tdex.network/tdex-sdk.html), but in the future, TDEX will have SDKs for Python, Go, and Rust. On the other hand, in the initial phase, traders interact with Providers using the [Command Line Interface](https://docs.tdex.network/tdex-cli.html#install) (CLI), until the future plan for a decentralised, mobile application comes to fruition.

Essentially, these SDKs represent TDEX&#39;s contributions to the network&#39;s open-source capabilities, primarily by empowering developers versed in bitcoin API implementation and other similar functionalities. In this regard, the broader vision is to drive innovations within the Liquid ecosystem, especially with the aim of strengthening liquidity generation on the network.

### 3.4 Use Cases

Having discussed the various elements of the TDEX ecosystem, let us now look at some of the prominent and possible use cases.

#### 3.4.1 Secondary Market for Liquid Assets

In general, it must be borne in mind that assets traded on the TDEX network are essentially Liquid Assets. Thus, being a secondary market for L-Assets is among the primary use cases of the TDEX platform, at least in the initial stages.

Briefly, Liquid allows its users to &quot;issue&quot; transferable assets, ranging across asset classes—tokenised fiat and other non-BTC cryptocurrencies, non-fungible tokens (collectibles), incentivisation tokens (rewards), tokenised commodities (for instance, gold coins), and so on. Every L-Asset has a 64-character identifier, which can be attached with human-readable domains on the blockchain by publishing their metadata on the &quot;Asset Registry&quot; at Blockstream.info—that is, on Liquid&#39;s version of a Block Explorer. The protocol also allows for reissuance tokens and token burns. In TDEX&#39;s context, this means that Providers can create markets for any pair of L-Assets, thus facilitating trades in these assets. Similarly, it could be leveraged for NFT transactions and sales.

At this point, however, it&#39;s imperative to note a crucial aspect of TDEX&#39;s vision—TDEX shall have no native token, primarily because the project is community-oriented and does not prioritise any profit-making motives.

#### 3.4.2 Institutional Trading &amp; Fund Transfer

Traders and Market Makers on the TDEX network need not necessarily be individuals, but can also be institutions and businesses. Thus, the platform provides a secure channel for such an organisation to trade in L-Assets, which in turn, should play a determining role in enhancing long-term adoptions and in extending the community.

Alongside this, TDEX&#39;s open-source toolkit further widens the scope by establishing the possibility for business—small, medium, and large—to deploy custom solutions to meet their financial needs in a decentralised manner. In fact, it is in this sense that TDEX&#39;s aim to become a &quot;backbone network&quot; for LiFi can be realised

## 4. Conclusion

Privacy and security concerns are mushrooming. Compliance obligations are crippling centralised exchanges in several ways, while the decentralised ones are compromising on security and falling prey to rampant hacks, scams, and breaches of several kinds. Ultimately, as a combined effect of these factors, users are either losing their money or their data, and more importantly, are being deprived of their basic rights to privacy and autonomy.

Developed against this backdrop, TDEX is a privacy-prioritised, decentralised solution deployed on the Liquid Network. Primarily an atomic-swap-based trading protocol, the platform also has an open-source toolkit that developers can use to deploy custom APIs and other solutions on the network. As a whole, TDEX envisions becoming a backbone protocol facilitating decentralised solutions on the Liquid Network, and in turn, strengthening the foundation of Liquid Finance (LiFi) as a secure, safe, and meritocratic space for a global community of crypto users and enthusiasts.

## Acknowledgments

Embarking on a journey towards building the future, TDEX has been inspired, advised, and assisted by several people and companies. Realising that the project would never be possible without them, we wish to acknowledge some of the many contributions.

[Blockstream](https://blockstream.com/)

[Vulpem Ventures](https://vulpem.com/)

[Mohammad Musharraf](http://mohammadmusharraf.com/)

[Shiladitya Sinha](https://www.linkedin.com/in/shiladityasinhaofficial/)
