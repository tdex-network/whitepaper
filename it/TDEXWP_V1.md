# TDEX: Una visione decentralizzata per sfruttare gli Atomic Swap nella Liquid Finance (LiFi)

**TDEX white paper | Version 1.0 | October 2020**

**Sommario:** TDEX (True DEX) è la prima piattaforma di scambi decentralizzati (Decentralised Exchange - DEX) basata su atomic swap, in grado di tutelare la privacy e realizzata su Liquid Network. Trattandosi di una soluzione open-source che si rivolge alla comunità, il suo obiettivo è quello di diventare il punto di riferimento per i cripto-utenti che intendono operare in un cyberspazio rapido e sicuro, oltre a fungere da mercato secondario per i Liquid Asset. A questo scopo, TDEX intende favorire la generazione di liquidità in modo da sfruttare la sicurezza dei Bitcoin e ridurre concretamente le loro difficoltà di fungibilità e privacy, consolidando allo stesso tempo le fondamenta della Liquid Finance (LiFi), la versione di Finanza Decentralizzata (Decentralised Finance - DeFi) di Liquid Network. In questo white paper, descriveremo l'ecosistema di tale progetto e la visione che ne costituisce il fondamento e illumina il percorso da seguire.

## 1. Introduction

Technological innovations are pivotal to human progress, and more often than not, they save and make lives better. Considering its immense significance, technology should ideally be accessible to all, equally and adequately. Yet, that hasn't been the case.

Focusing on the finance sector, one cannot deny that innovations in FinTech have substantially enhanced the overall end-user experience: one-touch payments, digital passbooks, e-KYC, and so on. However, although the acquired ease-of-use supposedly drives wider usage, in reality, traditional financial systems have been structurally exclusive of the global unbanked population of around [1.7 billion](https://globalfindex.worldbank.org/chapters/unbanked) adults.

Privacy, on the other hand, has been drastically violated. Governmental institutions and for-profit corporations not only pry into the user's online activities, but also misuse their personal data to monitor, censor, and advertise. Arguably, this amounts to an infringement of a very basic right of the user.

Primarily, this is a direct outcome of the involvement of multiple intermediaries like banks, governments, agents, brokers, and so on. These intermediaries serve as the overseers or "trust", and in the process, emerge as central points of control.

### 1.1 Bitcoin: Combining User-Oriented Technology

In 2008, Satoshi Nakamoto released the Bitcoin [white paper](https://nakamotoinstitute.org/bitcoin/), presenting a combination of four potent, *user-oriented* technologies—blockchain, cryptography, proof-of-work, and peer-to-peer—in the sense that they reinstate control with users, rather than with centralised governing entities. The innovation facilitated a new economic paradigm for secure, peer-to-peer monetary transactions within a distributed and fully-decentralised ecosystem. By tackling the problem of double-spending without using the trust-based model, Satoshi effectively eliminated third-party intermediaries from the process and replaced them with a computerised algorithm.

Tuttavia, nonostante abbiano tutte le caratteristiche del sound money e della riserva di valore, i Bitcoin, nella loro forma essenziale, non hanno mantenuto le loro promesse di privacy e fungibilità. In altre parole, le transazioni Bitcoin non sono anonime ma pseudonime, mentre la loro fungibilità è messa in discussione dall'analisi della chain e problemi simili. Inoltre, per ottimizzare la sicurezza e la resilienza delle operazioni, il nucleo del sistema Bitcoin scende a compromessi essenziali in nome della scalabilità, rivelandosi inefficiente per diverse soluzioni e funzionalità basate su criptovalute. Più avanti in questo articolo, vedremo come la sidechain Liquid cerca di risolvere questi problemi del Layer-1 di Bitcoin.

### 1.2 The Problem of Generating Consistent Value

Over the past decade, the community has become overcrowded and almost saturated with crypto-assets. Backed by disruptive promises, these assets have rapidly become popular. Yet, given the mammoth losses conceded to scams, hacks, and failed projects, one must critically examine whether a majority of these endeavours actually contribute towards the community's long-term progress. More importantly, how do they fare in terms of the domain's foundational principles?

**Exchange Centralizzati**. Per garantire un confronto coerente con gli obiettivi immediati del sistema TDEX, prendiamo in considerazione i mercati centralizzati che attualmente rappresentano il gateway principale per interagire con la maggior parte dei cripto-asset. Per soddisfare gli obblighi normativi e garantire la liquidità, la maggior parte delle piattaforme di scambio offrono servizi basati sulla custodia: mantengono il controllo sui fondi dell'utente e sulle chiavi private dei wallet del loro exchange.

A majority of custodial exchanges are owned, managed, and governed by singular entities, while funds and data are stored in centralised servers. Consequently, to trade and transact on these exchanges, users must interact with such siloed servers that represent a *single-point-of-failure*, thus exposing them to high risks of security and privacy breaches, censorship, as well as fund loss.

**Exchange decentralizzati**. In alternativa agli exchange centralizzati, si sono sviluppati numerosi servizi di exchange decentralizzati. In generale, essi implementano protocolli per la realizzazione di algoritmi di market making, comunemente noti come *Automated Market Maker* o AMM. Tali sistemi determinano automaticamente i prezzi attraverso metriche che misurano l'andamento di domanda-offerta, senza interferenze di terzi. Tuttavia, anche tali soluzioni presentano una serie di rischi, tra i quali i problemi di scalabilità sono i più importanti per le finalità discusse in questo documento.

Partially because of their underlying blockchains and also as a downside of implementing smart contracts, a majority of DEXs are non-scalable, thus resulting in very high transaction fees in periods of network congestion. In their present form, as a DEX becomes more popular, it also becomes infinitely costlier. Furthermore, bugs in smart contracts have emerged as a common peril for the industry, leading to users suffering substantial losses from hacks and breaches.

### 1.3 The TDEX Project

Sviluppato da SevenLabs, TDEX è un exchange decentralizzato basato su elementi e rivolto alla comunità, realizzato sulla Liquid Network. Sfruttando la sicurezza, la fungibilità e la velocità del framework combinato Bitcoin-Liquid, TDEX intende implementare un'esperienza di trading veloce, sicura e veramente decentralizzata per operare con i Liquid Asset (L-Assets).

The underlying TSWAP protocol implements atomic swaps and solves the liquidity problem through several "zero-to-one" incentives. TDEX also empowers liquidity providers by enabling them to choose their market-making strategy. On the other hand, traders gain from competitive rates, faster settlements, lower slippage, and better security.

Nelle sezioni seguenti, discuteremo tutti gli elementi principali e secondari della piattaforma TDEX. Nel processo, evidenzieremo come la piattaforma potrebbe agire da backbone per il sistema Liquid Finance (LiFi), consentendo ai trader professionisti e a gestori di imprese di operare, effettuare transazioni e investire in un ambiente che privilegia la privacy.

## 2. The Framework: Security, Privacy, and Speed

Sfruttando un core basato su Elements, TDEX opera sulla Liquid Network. In quanto sidechain di Bitcoin, Liquid ne eredita ed estende la sicurezza, migliorando al contempo gli aspetti di privacy, fungibilità e scalabilità. In questo sezione, spieghiamo i motivi che hanno portato ad adottare Liquid Network come infrastruttura di riferimento per TDEX.

Per risolvere efficacemente i problemi del trading decentralizzato sopra descritti, TDEX prevede una soluzione olistica che copre due aspetti. Da una parte, deve risolvere alcune delle preoccupazioni fondamentali della comunità di utenti, come la latenza, la privacy insufficiente e i problemi di fungibilità. Dall'altra parte, deve ampliare l'orizzonte delle soluzioni finanziarie open, consentendo nuove funzionalità rispetto al Layer 1 di Bitcoin. In altre parole, TDEX intende diversificare lo scopo del Layer 1 di Bitcoin ed è proprio su questo punto che la sua visione si congiunge a quella di Liquid, una sidechain bitcoin.

Come giustamente evidenziato dagli autori del [white paper](https://blockstream.com/assets/downloads/pdf/liquid-whitepaper.pdf) della Liquid Network, *"per il mondo ad alta velocità dei trader di criptovalute, le commissioni di transazione, le variazioni dei tempi di settlement, la trasmissione pubblica delle transazioni, nonché i rischi di riorganizzazione della chain, possono determinare costi significativi durante le loro attività di trading."*

A parte il consenso Byzantine Fault Tolerant (BFT) delle reti di cui tratteremo brevemente più avanti, l'implementazioni di transazioni confidenziali e l'emissione di asset sembravano essere le migliori per le finalità di TDEX.

### 2.1 The Strong Federation & Liquid's BFT Consensus

In parole semplici, Liquid sfrutta un meccanismo peg-in-peg-out, garantito da un insieme di "funzionari" *distribuiti a livello globale e culturale*, che nel loro complesso costituiscono una "[Strong Federation](https://blockstream.com/strong-federations.pdf)" di operatori. Per garantire che tali funzionari siano *personalmente coinvolti nella partita*, il protocollo richiede che tali soggetti siano titolari di exchange, broker e simili, cioè soggetti che abbiano forti motivazioni  a garantire la stabilità e lo sviluppo della rete Bitcoin. La federazione costituita da tali funzionari firma blocchi, transazioni e i cosiddetti *peg* su Liquid usando dei "moduli chiave", che impiegano una logica algoritmica per impedire transazioni e fork non autorizzati sulla critpovaluta. Inoltre il sottostante algoritmo di consenso BFT implementa uno *schema di commit in tre fasi di tipo round-robin* in cui i blocchi sono firmati ogni minuto per prevenire il rischio di riorganizzazioni della chain.

A differenza della *distribuzione casuale di Poisson* utilizzata dall'algoritmo di consenso PoW di Bitcoin, il sistema di peg bidirezionale federato adottato da Liquid implica notevoli miglioramenti nella latenza delle transazioni. A sua volta, ciò consente il settlement di transazioni e operazioni quasi in tempo reale (circa 2 minuti) sulla rete TDEX, preservando il carattere decentralizzato della piattaforma, poiché la federazione è un insieme di partecipanti che non sono reciprocamente affidabili. Inoltre, Liquid adotta un vettore di soglia, , dove *n* è il numero totale di funzionari e *k* rappresenta il numero minimo di firme necessarie affinché un blocco sia considerato valido. Nonostante il fatto che ogni funzionario deve avere un orologio adeguatamente sincronizzato, detto vettore consente alla rete di raggiungere maggiore *sicurezza* ed *efficacia*, che alla fine si traducono in una maggiore sicurezza e disponibilità di TDEX.

### 2.2 Confidential Transactions

Nel processo di sviluppo di TDEX, la consapevolezza che la privacy è un diritto umano fondamentale si è presentata come valore alla base della maggior parte delle scelte. Il registro pubblico di Bitcoin registra ogni transazione senza collegarla direttamente al mittente e, apparentemente, questo appare sufficiente a garantirne la privacy. Tuttavia, uno sguardo più attento rivela che la *pseudonimia* in misura considerevole non riesce a garantire l'*autonomia* dell'utente. Ad esempio, l'*analisi della blockchain* e il tracciamento della cronologia delle transazioni relative a una determinata chiave pubblica potrebbero effettivamente negare la pseudonimia dell'utente. Inoltre, gli schemi individuati nel processo potrebbero essere utilizzati anche per classificare le valute in *buone* e *cattive*, il che rappresenta una minaccia alla *fungibilità*. Attualmente, sono in fase di sviluppo delle soluzioni per risolvere questi problemi, e una di tali soluzioni è l'implementazione di TDEX.

One must note that privacy isn't merely about *secrecy*—rather, it implies that the user controls *if and when* to reveal a certain piece of information about themselves. In this regard, Liquid enhances Bitcoin's privacy metrics, and thus, again, its path intersects with TDEX's journey.

Implementing components such as *homomorphic commitments*, *Diffie-Hellman key exchange*, and *range proofs*, among others, Liquid enables "[Confidential Transactions](https://blockstream.com/bitcoin17-final41.pdf)'' wherein both the amount and the asset type are blinded. In other words, the amount and type of the asset being transacted is encrypted in a way such that it can neither be decrypted (opened) using another value, nor can it be determined given the commitment. Presuming the *Unspent Transaction Output* (UTXO) model, this method proves the validity of a transaction by proving that the _ **total input = total output** _, meaning that there has been no inflation, destruction, or double-spending in the process. Furthermore, the network leverages *Asset Surjection Proof* (ASP)—a form of Zero-Knowledge Proofs wherein, to put it simply, the '*asset tag*' proves that it is committed to a *spent asset*, but doesn't reveal which one.

As a primary cogwheel in Liquid's machine, confidential transactions adopt asymmetric encryptions using *blinding keys*—that is, a private-public key pair. Among other outcomes, it minimises the risks of interception during the key exchange process, thus making transactions optimally private and censorship-resistant. In simple terms, the process may be summarised as follows:

- The asset owner (sender), say Marie, broadcasts the public address for her intended transaction (swap). Understandably, this is visible to the entire network.
- An interested receiver, say Alice, *encodes her public blinding key* into an address which she shares with Marie. In the case of TSWAP, this exchange occurs over an encrypted messaging protocol which, apart from ensuring security, also enables both parties to verify the UTXOs involved in the transaction.
- Upon receiving the message, Marie builds the transaction and encrypts it with Alice's public address. Alice (the receiver) is the only person with the associated private key for this transaction, and thus, she alone can decrypt the transaction after it is recorded on the blockchain—not even Marie.

Consequently, the network addresses such transactional needs where a blanket "transparency" is rather undesirable. For instance, confidential transactions enable businesses to conduct financial processes in a way that is decentralised and verifiable, but simultaneously protects sensitive information from public exposure. Similarly, the principle strengthens the impetus for crypto adoption in other relevant sectors, such as governmental finance, and so on.

## 3. The TDEX Ecosystem

Il diffondersi di soluzioni decentralizzate sulla rete Liquid, o, come la chiama Adam Back, CEO di Blockstream, Liquid Finance o LiFi, ha recentemente acquisito una forza crescente. Di conseguenza, tale rete sta generando una quantità sempre crescente di valori, soprattutto sotto forma di Liquid Assets. A sua volta, TDEX tenta di soddisfare la crescente domanda da parte della comunità di un mercato secondario decentralizzato per questi asset, oltre a rappresentare uno strumento open source per promuovere ulteriormente l'innovazione.

Nelle sezioni precedenti, abbiamo discusso il quadro di riferimento di TDEX e le motivazioni alla base di alcune delle sue scelte cardine. Ora, approfondiremo l'ecosistema delle piattaforme, presentando al lettore una panoramica dei protocolli e delle implementazioni.

### 3.1 The Technical Pillars: Basics of True DEX (BOTD)

Il cuore di TDEX è rappresentato da quattro protocolli: *Message*, *&nbsp;Transport, Swap* e *&nbsp;Trade*, di cui ci occuperemo in questa sezione. Tuttavia, a questo proposito, il presente articolo evita volutamente di esporre descrizioni tecniche complete, che sono riportate nella documentazione tecnica disponibile nel repo [Specifiche TDEX](https://specs.tdex.network/).

#### 3.1.1 Message Protocol: BOTD #1

Un requisito fondamentale, diremmo primitivo, per la rete decentralizzata di TDEX è quello di offrire un canale sicuro per scambio di messaggi bidirezionali per collegare le controparti interessate. Tale connessione deve essere affidabile, stabile, peer-to-peer (P2P), ma soprattutto in grado di garantire la privacy. Sfruttando Liquid, TDEX può soddisfare questi requisiti per garantire *comunicazioni riservate*. Inoltre, per mettere in serie questi messaggi, TDEX implementa i *&nbsp;Protocol Buffers* di Google, un metodo indipendente dalla piattaforma e dal linguaggio per serializzare dati strutturati.

#### 3.1.2 Transport Protocol: BOTD #2

Per effettuare transazioni sulla rete, i daemon (gli utenti) necessitano canali di trasporto P2P, in cui si applicano le stesse esigenze di riservatezza e sicurezza del message protocol. A questo proposito, TDEX fornisce diverse opzioni con un diverso grado di privacy che l'utente può implementare separatamente o in congiunzione: *Clear Text{* (non sicuro), *Onion Service* (onion), *Server-Side TLS* (TLS), *Mutual TLS* (mTLS ) e *Noise_XK_secp256k1_ChaChaPoly_SHA256* (noise). Durante la partecipazione alla rete TDEX, gli utenti devono dichiarare il canale di trasporto da loro implementato.

#### 3.1.3 Swap Protocol: BOTD #3

Il protocollo TSWAP è un'implementazione sicura basata su atomic swap che consente a soggetti peer sulla rete di scambiare messaggi e transazioni firmati. In qualità di mezzo di collegamento tra il **&nbsp;Proposer** e il **&nbsp;Responder**, TSWAP è un elemento fondamentale dell'ecosistema TDEX. Sfruttando i suddetti protocolli, TSWAP ha quattro sotto-elementi principali:

- **SwapRequest:**  **t**** he proposer** initiates the swap.
- **SwapAccept:** the responder accepts the request.
- **SwapComplete:** the proposer confirms the secure connection.
- **SwapFail:** either party announces the swap's termination upon failure. In the future, an additional element—_failure_code—_could be implemented to denote the reason behind the failure.

#### 3.1.4 Trade Protocol: BOTD #4

Si tratta dell'implementazione più importante per TDEX. Il protocollo di trading combina tutti i precedenti BOTD per definire l'interfaccia pubblica che implementa il servizio di scambi senza custodia. A differenza del modello order-book tipico degli scambi custodial, questo protocollo consente ai *trader* e ai *market maker* di collegarsi direttamente utilizzando degli atomic swap.

In una sezione successiva, parleremo dell'ecosistema per trader e liquidity provider. Al momento, basta dire che i market maker rappresentano daemon *sempre attivi* e forniscono liquidità proporzionale ai valori della coppia di asseti **Base-Valutazione**. In futuro, TDEX adotterà contratti basati su [Simplicity](https://blockstream.com/simplicity.pdf) per migliorare ulteriormente la sicurezza e la privacy della piattaforma e consentire funzionalità più ampie.

### 3.2 TDEX for Market Makers

Sulla rete TDEX, i *Market Maker* sono quei soggetti che forniscono liquidità a coppie di asset scambiabili sull'exchange e quindi possono anche essere chiamati *Liquidity Providers* ( **Provider** ). La funzione principale del provider è quella di detenere una coppia sempre reciprocamente legata, costituita da un asset di valutazione (quote_asset) e un asset di base (base_asset). Tuttavia,  questo meccanismo si applica a qualsiasi coppia di asset e non necessariamente a quelle relative ai Bitcoin.

As a solution for the classic problem of [*Double Coincidence of Wants*](https://www.oxfordreference.com/view/10.1093/oi/authority.20110803095622703), TDEX enables market markers to run *always-on* endpoints, while also revealing its publicly reachable address using either of the channels defined in BOTD #2. This ensures readily available markets for the traders, thus addressing one of the major pain-points of decentralised exchanges.

#### 3.2.1 Implementazione del daemon

Per partecipare come Provider, occorre implementare un Daemon sulla rete eseguendolo tramite Docker o come Standalone (Scopri di più in: [ Procedura di implementazione dei daemon](https://docs.tdex.network/tdex-daemon.html)). Un daemon standard su TDEX dispone di due endpoint HTTP/2 gRPC: l'**interfaccia dei trader** (pubblica) e l'**interfaccia degli operatori** (privata). Mentre l'interfaccia pubblica rappresenta la porta per i trader (impostazione predefinita: 9945), l'interfaccia privata (impostazione predefinita: 9000) viene utilizzata per le transazioni interne del market maker. Inoltre, per garantire la massima sicurezza, ogni daemon ha un wallet [Blockstream Green](https://help.blockstream.com/hc/en-us/categories/900000056183-Blockstream-Green) o Liquid pre-integrato.

#### 3.2.2 Market Making Strategies

Uno degli elementi qualificanti di TDEX è che esso fornisce molteplici opzioni di market making per i fornitori, ampliando così in modo significativo il loro ambito di applicazione. In altre parole, TDEX consente ai market maker di scegliere o creare le proprie strategie, senza imporne una.

Per impostazione predefinita, il protocollo adotta una strategia CFMM (*Constant Function Market-Making*) per determinare i prezzi degli asset. Tuttavia, i market maker hanno anche la possibilità di implementare feed (esterni) *collegabili* utilizzando un'API personalizzata. Considerando che il coinvolgimento delle aziende come fondamentale per il successo di TDEX, le strategie di market making personalizzate sono tra le funzionalità più importanti della piattaforma, soprattutto perché sostengono allo stesso tempo la logica di scelta degli utenti. In altre parole, mentre i fornitori possono scegliere la loro strategia di prezzo, i trader, che alla fine sono i veri fruitori della piattaforma, hanno la possibilità di accettare o rifiutare queste strategie.

#### 3.2.3 Transaction Fee

While the *base_asset-quote_asset* reserve ratio shifts with every trade, TDEX ensures consistency in the overall market size by levying a minimal transaction fee on every trade and adding it to the reserves. Considering that arbitrage shall motivate a consistent transactional flow, in cases where the market maker implements an AMM-based strategy, the revenue generated from the fee should rise over time.

Parallelly, however, TDEX adopts the [P2EP](https://en.bitcoin.it/wiki/PayJoin)[mechanism](https://en.bitcoin.it/wiki/PayJoin), thus minimising the blockchain space required by transactions which effectively optimises the fee involved. This is done to ensure a fair and level playground for both Traders and Providers on the platform.

#### 3.2.4 Liquidity Pools (Implementazione futura)

Andando avanti nella roadmap prevista, TDEX intende implementare la funzionalità di un servizio *senza custodia* che può fungere da struttura di riferimento per il collegamento dei daemon e la condivisione delle loro risorse. Una volta realizzata, questa funzione garantirà una liquidità maggiore e più coerente sulla piattaforma, oltre a presentare un unico endpoint per maggiore comodità dei trader. In questo modo, TDEX sarà in grado di accomodare richieste di liquidita e scalare.

In quanto tale, il fornitore che crea un pool sarà il *Pool Master* e altri fornitori potranno unirsi alla *rete di servizi distribuiti* per consolidare liquidità. Come incentivo, il pool master avrà la capacità di determinare il prezzo base per gli asset del pool e i trader avranno accesso ai prezzi spot aggregati del provider. Per un dato asset, ogni fornitore può operare da solo o entrare a far parte di un pool, ma non può assumere entrambi i ruoli contemporaneamente.

### 3.3 TDEX for Traders

Nel contesto TDEX, il *mercato* è una qualsiasi coppia costituita da asset base e di valutazione che possono essere scambiati con un atomic swap. Come descritto nella sezione BOTD #3, un **Proposer** deve avviare gli swap su TDEX e, in alternativa, agire da Trader sulla rete. In altre parole, un trader su TDEX è qualsiasi utente che implementa completamente il protocollo di trading (BOTD #4). In tal modo, è possibile connettersi all'Interfaccia del Trader descritta in precedenza ( la porta pubblica del daemon del fornitore) e fare trading al prezzo di mercato stabilito.

In generale, il trading su TDEX è simile a qualsiasi altra operazione basata su atomic swap, il che significa che il trader può scambiare quantità uguali (in base al valore di mercato) di entrambi gli asset della coppia. Tuttavia, a differenza della maggior parte dei competitor sui altre reti, il quadro di riferimento di TDEX garantisce riservatezza, settlement più rapidi e slippage ridotti o nulli. Inoltre, essendo un servizio senza custodia, TDEX evita ai trader il rischio di perdere fondi a causa di hacking e violazioni della sicurezza.

#### 3.3.1 Kit di sviluppo software: il contributo open source di TDEX a LiFi

Oltre all'interfaccia utente predefinita, la piattaforma consente inoltre ai trader di implementare il proprio client personalizzato utilizzando i kit di sviluppo software (SDK) di TDEX. Nella fase iniziale, questo può essere fatto utilizzando [JavaScript](https://docs.tdex.network/tdex-sdk.html), ma in futuro TDEX disporrà di SDK per Python, Go e Rust. Nella fase iniziale, i trader interagiscono con i fornitori utilizzando l'[interfaccia della riga di comando](https://docs.tdex.network/tdex-cli.html#install) (CLI), fino a quando non sarà realizzato il futuro progetto di un'applicazione decentralizzata per dispositivi mobili.

Essentially, these SDKs represent TDEX's contributions to the network's open-source capabilities, primarily by empowering developers versed in bitcoin API implementation and other similar functionalities. In this regard, the broader vision is to drive innovations within the Liquid ecosystem, especially with the aim of strengthening liquidity generation on the network.

### 3.4 Use Cases

Dopo aver discusso i vari elementi dell'ecosistema TDEX, esaminiamo ora alcuni dei principali casi di utilizzo.

#### 3.4.1 Mercato secondario di Liquid Asset

In general, it must be borne in mind that assets traded on the TDEX network are essentially Liquid Assets. Thus, being a secondary market for L-Assets is among the primary use cases of the TDEX platform, at least in the initial stages.

In breve, Liquid consente ai suoi utenti di "emettere" asset trasferibili, appartenenti a varie classi: fiat tokenizzati e altre criptovalute diverse dai BTC, token non fungibili (asset collezionabili), token di incentivazione (premi), materie prime tokenizzate (ad esempio, monete d'oro), e così via. Ogni L-Asset ha un identificatore di 64 caratteri, che può essere associato a domini leggibili sulla blockchain tramite pubblicazione dei loro metadati sul "Registro degli asset" nel sito Blockstream.info, che è la versione Liquid di un Block Explorer. Il protocollo consente anche la riemissione di token e i token burn. Nell'ambito di TDEX, ciò implica che i fornitori possono creare mercati per qualsiasi coppia di L-Asset, facilitando così gli scambi di tali asset. Allo stesso modo, il sistema potrebbe essere sfruttato per transazioni e vendite NFT.

A questo punto, tuttavia, è indispensabile sottolineare un aspetto cruciale della visione di TDEX: TDEX non avrà token nativi, soprattutto perché il progetto è orientato alla comunità e non prevede fini di lucro.

#### 3.4.2 Institutional Trading & Fund Transfer

I trader e i market maker sulla rete TDEX non devono necessariamente essere singoli privati, ma possono anche essere istituiti e imprese. Pertanto, la piattaforma fornisce un canale sicuro alle organizzazioni di questi tipo che intendono operare su L-Asset. Cio' favorirà l'adozione a lungo termine di tale soluzione e il consolidamento della comunità di utenti.

Oltre a questo, il toolkit open source di TDEX amplia ulteriormente la flessibilità della soluzione, dando la possibilità ad aziende piccole, medie e grandi di implementare soluzioni personalizzate per soddisfare le proprie esigenze finanziarie in modo decentralizzato. Infatti, è in questo senso che TDEX punta a diventare una "backbone network" per LiFi

## 4. Conclusion

I problemi di privacy e sicurezza si moltiplicano. I numerosi obblighi di conformità rischiano di ostacolare gli scambi centralizzati in vari modi, mentre quelli decentralizzati ricorrono a compromessi sulla sicurezza e sono spesso vittima di dilaganti attacchi, truffe e violazioni di ogni tipo. In definitiva, come effetto combinato di questi fattori, gli utenti stanno perdendo i loro soldi o i loro dati e, soprattutto, si vedono privati dei loro diritti fondamentali alla privacy e all'autonomia.

TDEX è una sistema decentralizzato basato sulla privacy e implementato su Liquid Network, sviluppato proprio per offrire una soluzione alternativa in questo contesto. Si tratta essenzialmente di un protocollo di trading basato su atomic swap, ma la piattaforma dispone anche di un toolkit open source che gli sviluppatori possono utilizzare per distribuire API personalizzate e altre soluzioni di rete. Nel complesso, TDEX punta a diventare un protocollo di riferimento che facilita soluzioni decentralizzate su Liquid Network e, di conseguenza,  rafforzare le fondamenta della Liquid Finance (LiFi) come spazio sicuro, protetto e fondato sul merito per una comunità globale di utenti e appassionati di criptovalute.

## Acknowledgments

TDEX è stato ispirato, consigliato e seguito da molte persone e aziende durante questo viaggio verso la realizzazione di un futuro migliore. Siamo consapevoli che il progetto non sarebbe mai stato possibile senza il loro contributo, pertanto desideriamo  riconoscere alcuni di tali soggetti.

[Blockstream](https://blockstream.com/)

[Vulpem Ventures](https://vulpem.com/)

[Mohammad Musharraf](http://mohammadmusharraf.com/)

[Shiladitya Sinha](https://www.linkedin.com/in/shiladityasinhaofficial/)
