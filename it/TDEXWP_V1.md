# TDEX: Una visione decentralizzata per sfruttare gli Atomic Swap nella Trustless Finance

**White paper su TDEX | Versione 1.1 | Giugno 2022**

**Sommario:** TDEX (True DEX) è il primo progetto di scambi decentralizzati (Decentralised Exchange – DEX) basato su atomic swap, in grado di tutelare la privacy e realizzato su Liquid Network. Trattandosi di un progetto open-source che si rivolge alla comunità, il suo obiettivo è quello di diventare il punto di riferimento per gli utenti Bitcoin che intendono operare in un cyberspazio rapido e sicuro, oltre a fungere da mercato secondario per i Liquid Asset. A questo scopo, TDEX intende favorire la generazione di liquidità in modo da sfruttare la sicurezza dei Bitcoin e ridurre concretamente le loro difficoltà di fungibilità e privacy, consolidando allo stesso tempo le fondamenta della Trustless Finance. In questo white paper, descriveremo l'ecosistema di tale progetto e la visione che ne costituisce il fondamento e illumina il percorso da seguire.

## 1. Introduzione

Le innovazioni tecnologiche sono fondamentali per il progresso umano e, il più delle volte, salvano e migliorano la vita. Considerando il suo immenso significato, la tecnologia dovrebbe idealmente essere adeguatamente accessibile a tutti allo stesso modo. Tuttavia, non sempre le cose sono andate così.

Limitandoci al settore finanziario, non si può negare che le innovazioni nel settore FinTech hanno sostanzialmente migliorato l'esperienza complessiva degli utenti finali: pagamenti one-touch, libretti di risparmio digitali, strumenti di e-KYC e così via. Tuttavia, anche se la facilità di utilizzo raggiunta da tali strumenti ne determina apparentemente un utilizzo più ampio, in realtà, i sistemi finanziari tradizionali sono stati strutturalmente inaccessibili a una popolazione mondiale priva di servizi bancari di circa [1,7 miliardi](https://globalfindex.worldbank.org/chapters/unbanked) di adulti.

La privacy, d'altra parte, è stata violata sistematicamente. Gli enti governativi e le società a fini di lucro non solo si intromettono nelle attività online dell'utente, ma sfruttano anche i loro dati personali per svolgere attività di monitoraggio, controllo e pubblicità. Quasi certamente, tutto questo costituisce una violazione dei diritti fondamentali dell'utente.

Tutto questo è dovuto soprattutto al coinvolgimento di troppi intermediari come banche, governi, agenti, broker e altri soggetti di questo tipo. Questi intermediari fungono da supervisori o "soggetti fiduciari", che nel processo emergono come punti centrali di controllo.

### 1.1 Bitcoin: combinazione di tecnologie orientate all'utente

Nel 2008, Satoshi Nakamoto ha pubblicato il celebre [white paper](https://nakamotoinstitute.org/bitcoin/) sui Bitcoin, che presentava una combinazione di quattro potenti tecnologie *orientate all'utente:* blockchain, crittografia, strumenti proof-of-work e peer-to-peer. Tali tecnologie restituiscono il controllo delle operazioni agli utenti, senza il coinvolgimento di enti di governo centralizzati. L'innovazione ha facilitato l'introduzione di un nuovo modello economico che favorisce transazioni monetarie sicure di tipo peer-to-peer nell'ambito di un ecosistema distribuito e completamente decentralizzato. Aggirando il cosiddetto problema della doppia spesa senza ricorrere a modelli basati sull'attendibilità, Satoshi ha efficacemente eliminato la presenza di intermediari esterni dal processo, sostituendoli con un algoritmo computerizzato.

Tuttavia, nonostante abbiano tutte le caratteristiche del sound money e della riserva di valore, i Bitcoin, nella loro forma essenziale, non hanno mantenuto le loro promesse di privacy e fungibilità. In altre parole, le transazioni Bitcoin non sono anonime ma pseudonime, mentre la loro fungibilità è messa in discussione dall'analisi della chain e problemi simili. Inoltre, per ottimizzare la sicurezza e la resilienza delle operazioni, il nucleo del sistema Bitcoin scende a compromessi essenziali in nome della scalabilità, rivelandosi inefficiente per diverse soluzioni e funzionalità basate su criptovalute. Più avanti in questo articolo, vedremo come la sidechain Liquid cerca di risolvere questi problemi del Layer-1 di Bitcoin.

### 1.2 Il problema della generazione continua di valori

Negli ultimi dieci anni, il mercato è stato invaso e quasi saturato da cripto-asset. Quasi sempre accompagnati da promesse roboanti, questi asset sono rapidamente diventati  popolari. Tuttavia, date le enormi perdite registrate a seguito di truffe, hacking e progetti falliti, è necessario valutare criticamente se la maggior parte di questi tentativi abbia realmente contribuito al progresso a lungo termine della comunità. Ma soprattutto occorre chiedersi: tali strumenti rispettano i principi fondamentali del settore?

**Exchange Centralizzati**. Per garantire un confronto coerente con gli obiettivi immediati del sistema TDEX, prendiamo in considerazione i mercati centralizzati che attualmente rappresentano il gateway principale per interagire con la maggior parte dei cripto-asset. Per soddisfare gli obblighi normativi e garantire la liquidità, la maggior parte delle piattaforme di scambio offrono servizi basati sulla custodia: mantengono il controllo sui fondi dell'utente e sulle chiavi private dei wallet del loro exchange.

La maggior parte degli exchange con servizio di custodia è posseduta, gestita e governata da singole organizzazioni, mentre i fondi e i dati sono archiviati in server centralizzati. Di conseguenza, per operare ed effettuare transazioni su questi exchange, gli utenti devono interagire con tali server che costituiscono altrettanti *single-point-of-failure* (punti di vulnerabilità) ed espongono gli utenti ad elevati rischi di violazioni della sicurezza e della privacy, controlli indesiderati e perdite di fondi.

**Exchange decentralizzati**. In alternativa agli exchange centralizzati, si sono sviluppati numerosi servizi di exchange decentralizzati. In generale, essi implementano protocolli per la realizzazione di algoritmi di market making, comunemente noti come *Automated Market Maker* o AMM. Tali sistemi determinano automaticamente i prezzi attraverso metriche che misurano l'andamento di domanda-offerta, senza interferenze di terzi. Tuttavia, anche tali soluzioni presentano una serie di rischi, tra i quali i problemi di scalabilità sono i più importanti per le finalità discusse in questo documento.

In parte a causa delle loro blockchain sottostanti, ma anche come effetto collaterale dell'implementazione di smart contact, la maggior parte dei sistemi DEX non è scalabile, con conseguenti commissioni di transazione molto elevate nei periodi di congestione di rete. Nella loro forma attuale, quanto più un DEX si diffonde, tanto più diventa costoso. Inoltre, i bug negli smart contract si sono dimostrati punti di vulnerabilità comuni nel settore, portando gli utenti a subire perdite sostanziali a causa di hacking e violazioni.

### 1.3 Il progetto TDEX

Sviluppato da SevenLabs, TDEX è un exchange decentralizzato basato su elementi e rivolto alla comunità, realizzato sulla Liquid Network. Sfruttando la sicurezza, la fungibilità e la velocità del framework combinato Bitcoin-Liquid, TDEX intende implementare un'esperienza di trading veloce, sicura e veramente decentralizzata per operare con i Liquid Asset (L-Assets).

Il sottostante protocollo TSWAP implementa gli atomic swap e risolve il problema della liquidità attraverso diversi incentivi "zero-to-one". TDEX aiuta anche i fornitori di liquidità, consentendo loro di scegliere la propria strategia di market-making. D'altra parte, i trader guadagnano grazie a prezzi competitivi, settlement più rapidi, slippage ridotti e maggiore sicurezza.

Nelle sezioni seguenti, discuteremo tutti gli elementi principali e secondari del progetto TDEX. Nel processo, evidenzieremo come il protocollo potrebbe agire da backbone per il sistema Trustless Finance, consentendo ai trader professionisti e a gestori di imprese di operare, effettuare transazioni e investire in un ambiente che privilegia la privacy.

## 2. Lo schema di riferimento: sicurezza, privacy e velocità

Sfruttando un core basato su Elements, TDEX opera sulla Liquid Network. In quanto sidechain di Bitcoin, Liquid ne eredita ed estende la sicurezza, migliorando al contempo gli aspetti di privacy, fungibilità e scalabilità. In questo sezione, spieghiamo i motivi che hanno portato ad adottare Liquid Network come infrastruttura di riferimento per TDEX.

Per risolvere efficacemente i problemi del trading decentralizzato sopra descritti, TDEX prevede una soluzione olistica che copre due aspetti. Da una parte, deve risolvere alcune delle preoccupazioni fondamentali della comunità di utenti, come la latenza, la privacy insufficiente e i problemi di fungibilità. Dall'altra parte, deve ampliare l'orizzonte delle soluzioni finanziarie open, consentendo nuove funzionalità rispetto al Layer 1 di Bitcoin. In altre parole, TDEX intende diversificare lo scopo del Layer 1 di Bitcoin ed è proprio su questo punto che la sua visione si congiunge a quella di Liquid, una sidechain bitcoin.

Come giustamente evidenziato dagli autori del [white paper](https://blockstream.com/assets/downloads/pdf/liquid-whitepaper.pdf) della Liquid Network, *"per il mondo ad alta velocità dei trader di criptovalute, le commissioni di transazione, le variazioni dei tempi di settlement, la trasmissione pubblica delle transazioni, nonché i rischi di riorganizzazione della chain, possono determinare costi significativi durante le loro attività di trading."*

A parte il consenso Byzantine Fault Tolerant (BFT) delle reti di cui tratteremo brevemente più avanti, l'implementazioni di transazioni confidenziali e l'emissione di asset sembravano essere le migliori per le finalità di TDEX.

### 2.1 La Strong Federation e il Consenso BFT di Liquid

In parole semplici, Liquid sfrutta un meccanismo peg-in-peg-out, garantito da un insieme di "funzionari" *distribuiti a livello globale e culturale*, che nel loro complesso costituiscono una "[Strong Federation](https://blockstream.com/strong-federations.pdf)" di operatori. Per garantire che tali funzionari siano *personalmente coinvolti nella partita*, il protocollo richiede che tali soggetti siano titolari di exchange, broker e simili, cioè soggetti che abbiano forti motivazioni  a garantire la stabilità e lo sviluppo della rete Bitcoin. La federazione costituita da tali funzionari firma blocchi, transazioni e i cosiddetti *peg* su Liquid usando dei "moduli chiave", che impiegano una logica algoritmica per impedire transazioni e fork non autorizzati sulla critpovaluta. Inoltre il sottostante algoritmo di consenso BFT implementa uno *schema di commit in tre fasi di tipo round-robin* in cui i blocchi sono firmati ogni minuto per prevenire il rischio di riorganizzazioni della chain.

A differenza della *distribuzione casuale di Poisson* utilizzata dall'algoritmo di consenso PoW di Bitcoin, il sistema di peg bidirezionale federato adottato da Liquid implica notevoli miglioramenti nella latenza delle transazioni. A sua volta, ciò consente il settlement di transazioni e operazioni quasi in tempo reale (circa 2 minuti) sulla rete TDEX, preservando il carattere decentralizzato del protocollo, poiché la federazione è un insieme di partecipanti che non sono reciprocamente affidabili. Inoltre, Liquid adotta un vettore di soglia, , dove *n* è il numero totale di funzionari e *k* rappresenta il numero minimo di firme necessarie affinché un blocco sia considerato valido. Nonostante il fatto che ogni funzionario deve avere un orologio adeguatamente sincronizzato, detto vettore consente alla rete di raggiungere maggiore *sicurezza* ed *efficacia*, che alla fine si traducono in una maggiore sicurezza e disponibilità di TDEX.

### 2.2 Transazioni confidenziali

Nel processo di sviluppo di TDEX, la consapevolezza che la privacy è un diritto umano fondamentale si è presentata come valore alla base della maggior parte delle scelte. Il registro pubblico di Bitcoin registra ogni transazione senza collegarla direttamente al mittente e, apparentemente, questo appare sufficiente a garantirne la privacy. Tuttavia, uno sguardo più attento rivela che la *pseudonimia* in misura considerevole non riesce a garantire l'*autonomia* dell'utente. Ad esempio, l'*analisi della blockchain* e il tracciamento della cronologia delle transazioni relative a una determinata chiave pubblica potrebbero effettivamente negare la pseudonimia dell'utente. Inoltre, gli schemi individuati nel processo potrebbero essere utilizzati anche per classificare le valute in *buone* e *cattive*, il che rappresenta una minaccia alla *fungibilità*. Attualmente, sono in fase di sviluppo delle soluzioni per risolvere questi problemi, e una di tali soluzioni è l'implementazione di TDEX.

Occorre notare che la privacy non è solo una questione di *segretezza*, ma implica che l'utente abbia la possibilità di decidere *se e quando* rivelare una certa informazione che lo riguarda. A questo proposito, Liquid migliora le metriche di privacy di Bitcoin e quindi, ancora una volta, il suo percorso si incrocia con il viaggio di TDEX.

Grazie all'implementazione di componenti quali *commitment omomorfi*, *scambi di chiavi Diffie-Hellman* e *range proof*, Liquid permette l'esecuzione di "[Transazioni confidenziali](https://blockstream.com/bitcoin17-final41.pdf)'' il cui tipo di asset e importo sono davvero protetti. In altri termini, l'importo e il tipo di asset della transazione sono crittografati in modo da non poter essere decodificati (aperti) usando altri valori e da non poter essere individuati una volta dato il commitment. Assumendo l'utilizzo del modello *Unspent Transaction Output* (UTXO), questo metodo prova la validità di una transazione provando che _ **input totale = output totale** _, il che indica che nel processo non ci sono stati fenomeni di inflazione, distruzione o doppia spesa del capitale. Inoltre, la rete sfrutta l'*Asset Surjection Proof* (ASP), un tipo di dimostrazione a conoscenza zero in cui, in parole semplici, il '*tag dell'asset*' dimostra che si tratta di un *asset impegnato*, senza rivelarne i dettagli.

Essendo uno degli ingranaggi primari della macchina Liquid, le transazioni confidenziali adottano tecniche di crittografia asimmetrica utilizzando *chiavi nascoste*, ovvero una coppia di chiavi pubblica-privata. Tra gli altri risultati, questi sistemi riducono al minimo i rischi di intercettazione durante il processo di scambio delle chiavi, rendendo così le transazioni perfettamente private e non controllabili. In termini semplici, il processo può essere riassunto come segue:

- Il proprietario dell'asset (il mittente), ad esempio Alice, trasmette l'indirizzo pubblico per la sua transazione (swap). Naturalmente, questa informazione è visibile all'intera rete.
- Un destinatario interessato, ad esempio Bob, *codifica la sua chiave pubblica nascosta* in un indirizzo che condivide con Alice. Nel caso di TSWAP, questo scambio avviene tramite un protocollo di messaggi crittografati che, oltre a garantire la sicurezza, consente anche a entrambe le parti di verificare gli UTXO coinvolti nella transazione.
- Dopo aver ricevuto il messaggio, Alice crea la transazione e la codifica con l'indirizzo pubblico di Bob. Bob (il destinatario) è l'unica persona con la chiave privata associata a questa transazione, e quindi l'unica a poter decifrare la transazione dopo che è stata registrata sulla blockchain; nemmeno Alice è in grado di farlo.

Di conseguenza, la rete risponde alle esigenze di tali transazioni in cui una "trasparenza" globale è indesiderabile. Ad esempio, le transazioni confidenziali consentono alle aziende di condurre i processi finanziari in modo decentralizzato e verificabile, ma allo stesso tempo proteggono la riservatezza delle informazioni sensibili. Inoltre, questo principio può incoraggiare l'adozione dei Bitcoin in altri settori rilevanti, come la finanza pubblica e simili.

## 3. L'ecosistema TDEX

Il diffondersi di soluzioni decentralizzate sulla rete Liquid, o, come la chiama Adam Back, CEO di Blockstream, Liquid Finance o LiFi, ha recentemente acquisito una forza crescente. Di conseguenza, tale rete sta generando una quantità sempre crescente di valori, soprattutto sotto forma di Liquid Assets. A sua volta, TDEX tenta di soddisfare la crescente domanda da parte della comunità di un mercato secondario decentralizzato per questi asset, oltre a rappresentare uno strumento open source per promuovere ulteriormente l'innovazione.

Nelle sezioni precedenti, abbiamo discusso il quadro di riferimento di TDEX e le motivazioni alla base di alcune delle sue scelte cardine. Ora, approfondiremo l'ecosistema dei protocolli, presentando al lettore una panoramica dei protocolli e delle implementazioni.

### 3.1 I pilastri tecnici: le fondamenta di True DEX (BOTD)

Il cuore di TDEX è rappresentato da quattro protocolli: *Message*, *&nbsp;Transport, Swap* e *&nbsp;Trade*, di cui ci occuperemo in questa sezione. Tuttavia, a questo proposito, il presente articolo evita volutamente di esporre descrizioni tecniche complete, che sono riportate nella documentazione tecnica disponibile nel repo [Specifiche TDEX](https://dev.tdex.network/docs/specs/index).

#### 3.1.1 Message Protocol: BOTD #1

Un requisito fondamentale, diremmo primitivo, per la rete decentralizzata di TDEX è quello di offrire un canale sicuro per scambio di messaggi bidirezionali per collegare le controparti interessate. Tale connessione deve essere affidabile, stabile, peer-to-peer (P2P), ma soprattutto in grado di garantire la privacy. Sfruttando Liquid, TDEX può soddisfare questi requisiti per garantire *comunicazioni riservate*. Inoltre, per mettere in serie questi messaggi, TDEX implementa i *&nbsp;Protocol Buffers* di Google, un metodo indipendente dalla piattaforma e dal linguaggio per serializzare dati strutturati.

#### 3.1.2 Transport Protocol: BOTD #2

Per effettuare transazioni sulla rete, i daemon (gli utenti) necessitano canali di trasporto P2P, in cui si applicano le stesse esigenze di riservatezza e sicurezza del message protocol. A questo proposito, TDEX fornisce diverse opzioni con un diverso grado di privacy che l'utente può implementare separatamente o in congiunzione: *Clear Text{* (non sicuro), *Onion Service* (onion), *Server-Side TLS* (TLS), *Mutual TLS* (mTLS ) e *Noise_XK_secp256k1_ChaChaPoly_SHA256* (noise). Durante la partecipazione alla rete TDEX, gli utenti devono dichiarare il canale di trasporto da loro implementato.

#### 3.1.3 Protocollo di swap: BOTD #3

Il protocollo TSWAP è un'implementazione sicura basata su atomic swap che consente a soggetti peer sulla rete di scambiare messaggi e transazioni firmati. In qualità di mezzo di collegamento tra il **&nbsp;Proposer** e il **&nbsp;Responder**, TSWAP è un elemento fondamentale dell'ecosistema TDEX. Sfruttando i suddetti protocolli, TSWAP ha quattro sotto-elementi principali:

- **SwapRequest:** il **proponente** inizia lo swap.
- **SwapAccept:** il risponditore accetta la richiesta.
- **SwapComplete:** il proponente conferma la connessione sicura.
- **SwapFail:** una delle due parti dichiara la conclusione dello swap a causa di un problema. In futuro si pensa di implementare un elemento aggiuntivo, *failure_code*, che indica il motivo del problema.

#### 3.1.4 Trade Protocol: BOTD #4

Si tratta dell'implementazione più importante per TDEX. Il protocollo di trading combina tutti i precedenti BOTD per definire l'interfaccia pubblica che implementa il servizio di scambi senza custodia. A differenza del modello order-book tipico degli scambi custodial, questo protocollo consente ai *trader* e ai *market maker* di collegarsi direttamente utilizzando degli atomic swap.

In una sezione successiva, parleremo dell'ecosistema per utenti e liquidity provider. Al momento, basta dire che i market maker rappresentano daemon *sempre attivi* e forniscono liquidità proporzionale ai valori della coppia di asset **Base-Valutazione**. In futuro, TDEX adotterà contratti basati su [Simplicity](https://blockstream.com/simplicity.pdf) per migliorare ulteriormente la sicurezza e la privacy della piattaforma e consentire funzionalità più ampie.

### 3.2 TDEX per Market Maker

Sulla rete TDEX, i *Market Maker* sono soggetti che forniscono liquidità a coppie di asset scambiabili sull'exchange e quindi possono anche essere chiamati *Liquidity Providers* ( **Provider** ). La funzione principale del provider è quella di detenere una coppia sempre reciprocamente legata, costituita da un asset di valutazione (quote_asset) e un asset di base (base_asset). Tuttavia,  questo meccanismo si applica a qualsiasi coppia di asset e non necessariamente a quelle relative ai Bitcoin.

Per risolvere il classico problema della [*doppia coincidenza delle volontà*](https://www.oxfordreference.com/view/10.1093/oi/authority.20110803095622703), TDEX consente ai market maker di eseguire endpoint *sempre attivi*, rivelando anche il proprio indirizzo raggiungibile pubblicamente tramite uno dei canali definiti in BOTD #2. Ciò garantisce la pronta disponibilità dei mercati ai trader, superando così uno dei principali punti deboli degli exchange decentralizzati.

#### 3.2.1 Implementazione del daemon

Per partecipare come Provider, occorre implementare un Daemon sulla rete eseguendolo tramite Docker o come Standalone (Scopri di più in: [ Procedura di implementazione dei daemon](https://docs.tdex.network/tdex-daemon.html)). Un daemon standard su TDEX dispone di due endpoint HTTP/2 gRPC: l'**interfaccia dei trader** (pubblica) e l'**interfaccia degli operatori** (privata). Mentre l'interfaccia pubblica rappresenta la porta per i trader (impostazione predefinita: 9945), l'interfaccia privata (impostazione predefinita: 9000) viene utilizzata per le transazioni interne del market maker. Inoltre, per garantire la massima sicurezza, ogni daemon ha un wallet [Blockstream Green](https://help.blockstream.com/hc/en-us/categories/900000056183-Blockstream-Green) o Liquid pre-integrato.

#### 3.2.2 Strategie di market making

Uno degli elementi qualificanti di TDEX è che esso fornisce molteplici opzioni di market making per i fornitori, ampliando così in modo significativo il loro ambito di applicazione. In altre parole, TDEX consente ai market maker di scegliere o creare le proprie strategie, senza imporne una.

Per impostazione predefinita, il protocollo adotta una strategia CFMM (*Constant Function Market-Making*) per determinare i prezzi degli asset. Tuttavia, i market maker hanno anche la possibilità di implementare feed (esterni) *collegabili* utilizzando un'API personalizzata. Considerando che il coinvolgimento delle aziende sarà fondamentale per il successo di TDEX, le strategie di market making personalizzate sono tra le funzionalità più importanti della piattaforma, soprattutto perché sostengono allo stesso tempo la logica di scelta degli utenti. In altre parole, mentre i fornitori possono scegliere la loro strategia di prezzo, i trader, che alla fine sono i veri fruitori della piattaforma, hanno la possibilità di accettare o rifiutare queste strategie.

#### 3.2.3 Commissioni di swap

Mentre il coefficiente di riserva *base_asset-quote_asset* si modifica ad ogni scambio, TDEX garantisce la coerenza della dimensione complessiva del mercato, imponendo una commissione di swap minima su ogni operazione e aggiungendola alle riserve. Considerando che l'arbitraggio deve favorire un flusso di transazioni continuo, nei casi in cui il market maker implementi una strategia basata su AMM, le entrate generate dalle commissioni dovrebbero aumentare nel tempo.

Allo stesso tempo, tuttavia, TDEX adotta il [meccanismo](https://en.bitcoin.it/wiki/PayJoin) [P2EP](https://en.bitcoin.it/wiki/PayJoin), riducendo così al minimo lo spazio blockchain richiesto dalle transazioni, in modo da ottimizzare efficacemente la commissione coinvolta. Questo permette di garantire uno svolgimento delle operazioni equo ed equilibrato sia per i trader che per i fornitori sul protocollo.

#### 3.2.4 Liquidity Pools (Implementazione futura)

Andando avanti nella roadmap prevista, TDEX intende implementare la funzionalità di un servizio *senza custodia* che può fungere da struttura di riferimento per il collegamento dei daemon e la condivisione delle loro risorse. Una volta realizzata, questa funzione garantirà una liquidità maggiore e più coerente sul protocollo, oltre a presentare un unico endpoint per maggiore comodità degli utenti. In questo modo, TDEX sarà in grado di accomodare richieste di liquidità e scalare.

In quanto tale, il fornitore che crea un pool sarà il *Pool Master* e altri fornitori potranno unirsi alla *rete di servizi distribuiti* per consolidare liquidità. Come incentivo, il pool master avrà la capacità di determinare il prezzo base per gli asset del pool e i trader avranno accesso ai prezzi spot aggregati del provider. Per un dato asset, ogni fornitore può operare da solo o entrare a far parte di un pool, ma non può assumere entrambi i ruoli contemporaneamente.

### 3.3 TDEX per trader

Nel contesto TDEX, il *mercato* è una qualsiasi coppia costituita da asset base e di valutazione che possono essere scambiati con un atomic swap. Come descritto nella sezione BOTD #3, un **Proposer** deve avviare gli swap su TDEX e, in alternativa, agire da Trader sulla rete. In altre parole, un trader su TDEX è qualsiasi utente che implementa completamente il protocollo di trading (BOTD #4). In tal modo, è possibile connettersi all'Interfaccia del Trader descritta in precedenza (la porta pubblica del daemon del fornitore) e fare trading al prezzo di mercato stabilito.

In generale, il trading su TDEX è simile a qualsiasi altra operazione basata su atomic swap, il che significa che il trader può scambiare quantità uguali (in base al valore di mercato) di entrambi gli asset della coppia. Tuttavia, a differenza della maggior parte dei competitor sui altre reti, il quadro di riferimento di TDEX garantisce riservatezza, settlement più rapidi e slippage ridotti o nulli. Inoltre, essendo un servizio senza custodia, TDEX evita agli utenti il rischio di perdere fondi a causa di hacking e violazioni della sicurezza.

#### 3.3.1 Kit di sviluppo software: il contributo open source di TDEX a LiFi

Oltre all'interfaccia utente predefinita, il protocollo consente agli utenti di implementare il proprio client personalizzato utilizzando i kit di sviluppo software (SDK) di TDEX. Nella fase iniziale, questo può essere fatto utilizzando [JavaScript](https://docs.tdex.network/tdex-sdk.html), ma in futuro TDEX disporrà di SDK per Python, Go e Rust. Nella fase iniziale, i trader interagiscono con i fornitori utilizzando l'[interfaccia della riga di comando](https://docs.tdex.network/tdex-cli.html#install) (CLI), fino a quando non sarà realizzato il futuro progetto di un'applicazione decentralizzata per dispositivi mobili.

In sostanza, questi SDK rappresentano i contributi di TDEX alle funzionalità open source della rete, soprattutto perché aiutano gli sviluppatori esperti nell'implementazione di API bitcoin e altre funzionalità simili. A questo proposito, l'obiettivo più ambizioso è quelli di rendere TDEX l'elemento trainante delle innovazioni all'interno dell'ecosistema Liquid, soprattutto con l'obiettivo di rafforzare i servizi per la generazione di liquidità sulla rete.

### 3.4 Casi di utilizzo

Dopo aver discusso i vari elementi dell'ecosistema TDEX, esaminiamo ora alcuni dei principali casi di utilizzo.

#### 3.4.1 Mercato secondario di Liquid Asset

In generale, occorre considerare che gli asset scambiati sulla rete TDEX sono essenzialmente Liquid Assets. Pertanto, trattandosi di un mercato secondario per L-Asset, questo sarà uno dei casi di utilizzo principali della piattaforma TDEX, almeno nelle sue fasi iniziali.

In breve, Liquid consente ai suoi utenti di "emettere" asset trasferibili, appartenenti a varie classi: fiat tokenizzati e altre criptovalute diverse dai BTC, token non fungibili (asset collezionabili), token di incentivazione (premi), materie prime tokenizzate (ad esempio, monete d'oro), e così via. Ogni L-Asset ha un identificatore di 64 caratteri, che può essere associato a domini leggibili sulla blockchain tramite pubblicazione dei loro metadati sul "Registro degli asset" nel sito Blockstream.info, che è la versione Liquid di un Block Explorer. Il protocollo consente anche la riemissione di token e i token burn. Nell'ambito di TDEX, ciò implica che i fornitori possono creare mercati per qualsiasi coppia di L-Asset, facilitando così gli scambi di tali asset. Allo stesso modo, il sistema potrebbe essere sfruttato per transazioni e vendite NFT.

A questo punto, tuttavia, è indispensabile sottolineare un aspetto cruciale della visione di TDEX: TDEX non avrà token nativi, soprattutto perché il progetto è orientato alla comunità e non prevede fini di lucro.

#### 3.4.2 Trading istituzionale e trasferimento di fondi

Gli utenti e i market maker sulla rete TDEX non devono necessariamente essere singoli privati, ma possono anche essere istituiti e imprese. Pertanto, la piattaforma fornisce un canale sicuro alle organizzazioni di questi tipo che intendono operare su L-Asset. Ciò favorirà l'adozione a lungo termine di tale soluzione e il consolidamento della comunità di utenti.

Oltre a questo, il toolkit open source di TDEX amplia ulteriormente la flessibilità della soluzione, dando la possibilità ad aziende piccole, medie e grandi di implementare soluzioni personalizzate per soddisfare le proprie esigenze finanziarie in modo decentralizzato. Infatti, è in questo senso che TDEX punta a diventare una "backbone network" per Trustless Finance

## 4. Conclusioni

I problemi di privacy e sicurezza si moltiplicano. I numerosi obblighi di conformità rischiano di ostacolare gli scambi centralizzati in vari modi, mentre quelli decentralizzati ricorrono a compromessi sulla sicurezza e sono spesso vittima di dilaganti attacchi, truffe e violazioni di ogni tipo. In definitiva, come effetto combinato di questi fattori, gli utenti stanno perdendo i loro soldi o i loro dati e, soprattutto, si vedono privati dei loro diritti fondamentali alla privacy e all'autonomia.

TDEX è un protocollo decentralizzato basato sulla privacy e implementato su Liquid Network, sviluppato proprio per offrire una soluzione alternativa in questo contesto. Si tratta essenzialmente di un protocollo di trading basato su atomic swap, ma la piattaforma dispone anche di un toolkit open source che gli sviluppatori possono utilizzare per distribuire API personalizzate e altre soluzioni di rete. Nel complesso, TDEX punta a diventare un protocollo di riferimento che facilita soluzioni decentralizzate su Liquid Network e, di conseguenza, rafforzare le fondamenta della Trustless Finance come spazio sicuro, protetto e fondato sul merito per una comunità globale di utenti e appassionati di Bitcoin.

## Riconoscimenti

TDEX è stato ispirato, consigliato e seguito da molte persone e aziende durante questo viaggio verso la realizzazione di un futuro migliore. Siamo consapevoli che il progetto non sarebbe mai stato possibile senza il loro contributo, pertanto desideriamo  riconoscere alcuni di tali soggetti.

[Blockstream](https://blockstream.com/)

[Vulpem Ventures](https://vulpem.com/)

[Mohammad Musharraf](http://mohammadmusharraf.com/)

[Shiladitya Sinha](https://www.linkedin.com/in/shiladityasinhaofficial/)

Un ringraziamento particolare a Satoshi Nakamoto
