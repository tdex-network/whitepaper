# TDEX : une vision décentralisée pour exploiter les swaps atomiques pour la finance liquide (LiFi)

**Livre blanc TDEX | Version 1.0 | Octobre 2020**

**Résumé :** T(True)DEX est la première plateforme d'échange décentralisé (DEX) du genre, basée sur l'échange atomique et privilégiant la protection de la vie privée, reposant sur le réseau Liquid. En tant que solution open-source orientée vers la communauté, elle vise à devenir le cadre d'un cyberespace rapide et sécurisé pour les utilisateurs de cryptos, ainsi qu'un marché secondaire pour les actifs liquides. Ce faisant, TDEX facilite la génération de liquidités d'une manière qui tire parti de la sécurité de Bitcoin mais atténue considérablement ses défauts de confidentialité et de fongibilité, renforçant ainsi les bases de la Liquid Finance (LiFi), la version du réseau Liquid de la finance décentralisée (DeFi). Dans ce livre blanc, nous détaillons l'écosystème du projet et la vision sous-jacente qui le guide.

## 1. Introduction

Les innovations technologiques sont essentielles au progrès humain et, le plus souvent, permettent de sauver et d'améliorer des vies. Compte tenu de son immense importance, la technologie devrait idéalement être accessible à tous, de manière égale et adéquate. Or, cela n'est pas le cas.

Si l'on se concentre sur le secteur financier, on ne peut nier que les innovations de la FinTech ont considérablement amélioré l'expérience globale de l'utilisateur final : paiements immédiats, livrets numériques, e-KYC, etc. Toutefois, bien que la facilité d'utilisation soit censée entraîner une utilisation plus courante, les systèmes financiers traditionnels ont en réalité exclu structurellement la population mondiale non bancarisée, soit environ [1,7 milliard](https://globalfindex.worldbank.org/chapters/unbanked) d'adultes.

La confidentialité, en revanche, a été gravement violée. Les institutions gouvernementales et les sociétés à but lucratif s'immiscent non seulement dans les activités en ligne des utilisateurs, mais utilisent également leurs données personnelles à mauvais escient pour surveiller, censurer et faire de la publicité. On peut dire que cela constitue une violation d'un droit très fondamental de l'utilisateur.

Ceci est principalement le résultat direct de l'implication de nombreux intermédiaires comme les banques, les gouvernements, les agents, les courtiers… Ces intermédiaires servent de superviseurs ou de « garants » et, ce faisant, deviennent des points de contrôle centraux.

### 1.1 Bitcoin : combiner les technologies orientées vers l'utilisateur

En 2008, Satoshi Nakamoto a publié le [livre blanc](https://nakamotoinstitute.org/bitcoin/) Bitcoin, présentant une combinaison de quatre technologies puissantes, *orientées vers l'utilisateur* - la blockchain, la cryptographie, la preuve de travail et le peer-to-peer - dans le sens où elles rendent le contrôle aux utilisateurs, plutôt qu'aux entités de gouvernance centralisées. Cette innovation a facilité un nouveau paradigme économique pour des transactions monétaires sécurisées, de pair à pair, au sein d'un écosystème distribué et entièrement décentralisé. En s'attaquant au problème des doubles dépenses sans utiliser le modèle basé sur la confiance, Satoshi a éliminé les intermédiaires du processus et les a remplacés par un algorithme informatisé.

Néanmoins, malgré toutes les caractéristiques d'une monnaie saine et d'une réserve de valeur, Bitcoin, dans sa forme la plus simple, n'est pas à la hauteur de sa promesse de confidentialité et de fongibilité. En d'autres termes, les transactions de Bitcoin sont pseudonymes et non anonymes, tandis que sa fongibilité est remise en question par l'analyse des chaînes, et ainsi de suite. En outre, pour obtenir une sécurité et une résilience optimales, le cœur de Bitcoin fait des compromis essentiels en matière d'évolutivité, ce qui le rend inefficace pour plusieurs solutions et fonctionnalités basées sur la cryptographie. Plus loin dans le document, nous examinons comment la sidechain Liquid aborde ces problèmes avec la couche 1 de Bitcoin.

### 1.2 Le problème de la création d'une valeur constante

Au cours de la dernière décennie, la communauté est devenue surpeuplée et presque saturée de crypto-actifs. Soutenus par des promesses disruptives, ces actifs sont rapidement devenus populaires. Pourtant, étant donné les pertes énormes dues aux escroqueries, aux piratages et aux projets ratés, il faut se demander de manière critique si la majorité de ces efforts contribuent réellement au progrès à long terme de la communauté. Plus important encore, comment s'en sortent-ils vis à vis des principes fondamentaux du domaine ?

**Échanges de dépôt**. Par souci de cohérence avec l'objectif immédiat de TDEX, prenons l'exemple des échanges centralisés qui sont actuellement la principale passerelle d'interaction avec la plupart des crypto-actifs. Pour répondre aux obligations réglementaires et garantir la liquidité, la plupart des plateformes d'échange sont de dépôt : elles conservent le contrôle des fonds de l'utilisateur, ainsi que des clés privées du portefeuille qu'elles hébergent.

La majorité des échanges de dépôt sont détenus, gérés et régis par des entités uniques, tandis que les fonds et les données sont stockés dans des serveurs centralisés. Par conséquent, pour échanger et effectuer des transactions sur ces échanges, les utilisateurs doivent interagir avec ces serveurs cloisonnés qui représentent un *point de défaillance unique*, les exposant ainsi à des risques élevés de failles de sécurité et de confidentialité, de censure et de perte de fonds.

**Échanges décentralisés**. Comme alternative aux échanges de dépôt, plusieurs échanges décentralisés se sont multipliés. En général, ils mettent en œuvre des protocoles de création de marché algorithmiques, communément appelés *Automated Market Makers* ou AMM, déterminant les prix grâce à des mesures de l'offre et de la demande, sans interférence de tiers. Cependant, ils comportent leurs propres risques, parmi lesquels les problèmes d'évolutivité sont les plus pertinents dans le contexte de cet article.

En partie à cause de leurs blockchains sous-jacentes et également comme inconvénient de la mise en œuvre de contrats intelligents, la majorité des DEX ne sont pas évolutifs, ce qui entraîne des frais de transaction très élevés en période de congestion du réseau. Dans leur forme actuelle, à mesure qu'un DEX devient plus populaire, il devient également infiniment plus coûteux. En outre, les bogues dans les contrats intelligents sont devenus un danger courant dans le secteur, entraînant des pertes substantielles pour les utilisateurs en raison de piratages et de failles.

### 1.3 Le projet TDEX

Développé par SevenLabs, TDEX est un échange décentralisé orienté sur la communauté, basé sur Elements et bâti sur le réseau Liquid. Tirant parti de la sécurité, de la convivialité et de la vitesse combinées du framework Bitcoin-Liquid, TDEX envisage une expérience de trading rapide, sécurisée et véritablement décentralisée dans les actifs liquides (L-Assets).

Le protocole TSWAP sous-jacent implémente des swaps atomiques et résout le problème de liquidité grâce à plusieurs incitations «zéro à un». TDEX donne également le pouvoir fournisseurs de liquidité en leur permettant de choisir leur stratégie de tenue de marché. D'un autre côté, les traders bénéficient de tarifs compétitifs, de règlements plus rapides, d'un glissement moindre et d'une meilleure sécurité.

Dans les sections suivantes, nous aborderons les éléments d'arrière-plan et de premier plan de la plateforme TDEX. Dans le processus, nous soulignons comment la plateforme pourrait émerger en tant que réseau principal pour la Liquid Finance (LiFi), permettant aux traders professionnels et aux propriétaires d'entreprise de gérer, traiter et investir dans un environnement où la confidentialité prime.

## 2. Le cadre : sécurité, confidentialité et rapidité

Grâce à un cœur basé sur Elements, TDEX est déployé sur le réseau Liquid. En tant que sidechain Bitcoin, Liquid hérite et améliore sa sécurité, tout en améliorant les aspects de confidentialité, de fongibilité et d'évolutivité. Dans ce segment, nous expliquerons le choix de Liquid comme cadre pour TDEX.

Pour résoudre efficacement les crises susmentionnées du trading décentralisé, TDEX envisage une solution holistique à deux volets. D'une part, il doit résoudre certaines des préoccupations primitives de la communauté, telles que la latence, le manque de confidentialité et les menaces à la fongibilité. D'autre part, il doit élargir l'horizon des solutions financières ouvertes, permettant de nouvelles fonctionnalités par rapport au cœur de Bitcoin. En d'autres termes, TDEX entend diversifier la finalité de la couche 1 de Bitcoin et c'est précisément sur ce point que sa vision se confond avec celle de Liquid, une sidechain bitcoin de couche 2.

Comme le soulignent à juste titre les auteurs du [livre blanc](https://blockstream.com/assets/downloads/pdf/liquid-whitepaper.pdf) Liquid, *« pour le monde à grande vitesse du trader de cryptomonnaie, les frais de transaction, les écarts dans les délais de règlement, les transactions diffusées publiquement, ainsi que les risques de réorganisations de la chaîne peuvent entraîner des coûts importants pendant leurs activités de trading. »*

Hormis le consensus Byzantine Fault Tolerant (BFT) du réseau dont nous parlerons brièvement, les implémentations telles que les transactions confidentielles et l'émission d'actifs semblaient être les plus pertinentes aux fins de TDEX.

### 2.1 La fédération forte et le consensus BFT de Liquid

Pour faire simple, Liquid fonctionne avec un mécanisme de peg-in-peg-out, sécurisé par un ensemble de « fonctionnaires » *répartis dans le monde entier et culturellement*, formant collectivement une «  [fédération forte](https://blockstream.com/strong-federations.pdf) » de validateurs. Pour que ces fonctionnaires *risquent leur peau*, le protocole exige qu'ils soient des échanges, des courtiers, etc., c'est-à-dire des entités ayant une motivation importante pour assurer la stabilité et le progrès du réseau Bitcoin. La fédération signe des blocs, des transactions et des *pegs* sur Liquid en utilisant des « modules clés » qui appliquent une logique algorithmique pour restreindre les forks et les transactions non autorisées. En outre, le consensus BFT sous-jacent met en œuvre un schéma de *validation round-robin en trois phases* et les blocs sont signés toutes les minutes, sans risque de réorganisation de la chaîne.

Contrairement à la *distribution aléatoire de Poisson* du consensus PoW de Bitcoin, l'ancrage bidirectionnel fédéré de Liquid implique de nombreuses améliorations de la latence transactionnelle. À son tour, cela permettrait un règlement des transactions et des transactions presque en temps réel (~ 2 minutes) sur le réseau TDEX, tout en préservant la décentralisation de la plateforme puisque la fédération est un ensemble de participants mutuellement non confiants. De plus, Liquid adopte un vecteur seuil,, où *n* est le nombre total de fonctionnaires et *k* représente le nombre minimum de signatures nécessaires pour qu'un bloc soit considéré comme valide. Nonobstant le fait que chaque fonctionnaire doit avoir une horloge correctement synchronisée, ledit vecteur permet au réseau d'atteindre à la fois la *sécurité* et la *vivacité*, ce qui se traduit finalement par une plus grande sécurité et une plus grande disponibilité pour TDEX.

### 2.2 Transactions confidentielles

Lors du développement de TDEX, la prise de conscience que la vie privée est un droit humain fondamental s'est présentée comme le substrat d'une majorité de choix. Le grand livre public de Bitcoin enregistre chaque transaction sans les lier directement à l'expéditeur, et apparemment, cela suffit pour la confidentialité. Cependant, un examen plus attentif révèle que le *pseudonymat*, dans une large mesure, ne garantit pas l'*autonomie* de l'utilisateur. Par exemple, l'*analyse de la chaîne* et le suivi de l'historique des transactions liées à une certaine clé publique pourraient effectivement annuler le pseudonymat de l'utilisateur. De plus, les modèles révélés au cours du processus pourraient également être utilisés pour classer les *bonnes* et les *mauvaises* pièces, ce qui constitue une menace pour la *fongibilité*. Des solutions sont actuellement en cours de développement pour résoudre ces problèmes, notamment l'implémentation de TDEX.

Il faut noter que la confidentialité n'est pas seulement une question de *secret*, mais plutôt que l'utilisateur contrôle *si et quand* révéler une certaine information sur lui-même. À cet égard, Liquid améliore la confidentialité de Bitcoin, et donc, encore une fois, son chemin croise le parcours de TDEX.

En mettant en œuvre des composants tels que les *engagements homomorphiques*, l'*échange de clés Diffie-Hellman*, et les *preuves de portée*, entre autres, Liquid permet des « [transactions confidentielles](https://blockstream.com/bitcoin17-final41.pdf) » où le montant et le type d'actif sont masqués. En d'autres termes, le montant et le type de l'actif faisant l'objet de la transaction sont chiffrés de telle sorte qu'il ne peuvent être ni déchiffrés (ouvert) en utilisant une autre valeur, ni déterminés grâce à l'engagement. En supposant le modèle *Unspent Transaction Output* (UTXO), cette méthode prouve la validité d'une transaction en démontrant que _ **l'entrée totale = la sortie totale** _, ce qui signifie qu'il n'y a pas eu d'inflation, de destruction ou de double dépense dans le processus. En outre, le réseau exploite la*preuve de surjection d'actif* (Asset Surjection Proof - ASP) - une forme de preuve de connaissance zéro dans laquelle, pour faire simple, la balise « *asset tag* » prouve qu'elle est engagée sur un *actif dépensé*, mais ne révèle pas lequel.

En tant que principal rouage de la machine de Liquid, les transactions confidentielles adoptent des chiffrements asymétriques utilisant des *clés aveugles,* c'est-à-dire une paire de clés privée-publique. Entre autres résultats, cela minimise les risques d'interception pendant le processus d'échange de clés, rendant ainsi les transactions privées et résistantes à la censure de manière optimale. En termes simples, le processus peut être résumé comme suit :

- Le propriétaire de l'actif (l'expéditeur), Marie par exemple, diffuse l'adresse publique de la transaction envisagée (échange). Naturellement, cela est visible sur l'ensemble du réseau.
- Un récepteur intéressé, disons Alice, *encode sa clé publique aveugle* dans une adresse qu'elle partage avec Marie. Dans le cas du TSWAP, cet échange se fait via un protocole de messagerie chiffré qui, en plus d'assurer la sécurité, permet également aux deux parties de vérifier les UTXO impliqués dans la transaction.
- À la réception du message, Marie construit la transaction et la chiffre avec l'adresse publique d'Alice. Alice (le destinataire) est la seule personne avec la clé privée associée pour cette transaction, et donc, elle seule peut déchiffre la transaction après son enregistrement sur la blockchain - pas même Marie.

Par conséquent, le réseau répond à ces besoins transactionnels là où une « transparence » générale est plutôt indésirable. Par exemple, les transactions confidentielles permettent aux entreprises de mener des processus financiers de manière décentralisée et vérifiable, tout en protégeant simultanément les informations sensibles de l'exposition publique. De même, le principe renforce l'élan en faveur de l'adoption des cryptos dans d'autres secteurs pertinents, tels que les finances gouvernementales, entre autres.

## 3. L'écosystème TDEX

L'émergence de solutions décentralisées sur le réseau Liquid - ou, comme Adam Back, le PDG de Blockstream, l'appelle, Liquid Finance ou LiFi - a gagné en force ces derniers temps. Par conséquent, une valeur croissante est générée sur le réseau, notamment sous forme d'actifs liquides. À son tour, TDEX s'efforce de répondre à la demande croissante de la communauté pour un marché secondaire décentralisé pour ces actifs, en plus d'être une boîte à outils open source pour favoriser davantage l'innovation.

Dans les sections précédentes, nous avons discuté du cadre de TDEX et des raisons derrière certains de ses choix cruciaux. Maintenant, nous développerons l'écosystème de la plateforme, en présentant au lecteur un aperçu des protocoles et des implémentations.

### 3.1 Les piliers techniques : principes de base du True DEX (BOTD)

Au cœur de TDEX, il existe quatre protocoles - *Message* , *Transport, Échange* et *Négociation* - dont nous parlerons dans ce segment. Cependant, à cet égard, le document s'abstient délibérément d'élaborer les expositions techniques complètes qui sont disponibles dans les documentations techniques dans les [Spécifications TDEX](https://specs.tdex.network/) .

#### 3.1.1 Protocole de message : BOTD # 1

Une exigence fondamentale, dite primitive, pour le réseau décentralisé de TDEX est un canal de messagerie bidirectionnel sécurisé pour connecter les contreparties. Une telle connexion doit être fiable, stable, peer-to-peer (P2P) et surtout, proriser la confidentialité. Grâce à Liquid, TDEX peut répondre à ces exigences en matière de *communications confidentielles*. De plus, pour sérialiser ces messages, TDEX implémente les *Tampons de protocole* Google, une plateforme et une méthode indépendante du langage pour la sérialisation de données structurées.

#### 3.1.2 Protocole de transport : BOTD # 2

Pour effectuer des transactions sur le réseau, les démons (utilisateurs) nécessitent des canaux de transport P2P, dans lesquels le besoin de confidentialité et de sécurité s'applique de la même manière que le protocole de message. À cet égard, TDEX fournit plusieurs options avec un degré de confidentialité variable que l'utilisateur peut implémenter soit de manière isolée, soit en combinaison : *Texte clair* (non sécurisé), *Service onion* (onion), *TLS serveur* (TLS), *TLS mutuel* (mTLS) ) et *Noise_XK_secp256k1_ChaChaPoly_SHA256* (bruit). Lors de leur participation au réseau TDEX, les utilisateurs doivent déclarer leur canal de transport implémenté.

#### 3.1.3 Protocole d'échange : BOTD # 3

Le protocole TSWAP est une implémentation sécurisée basée sur l'échange atomique permettant aux pairs du réseau d'échanger des messages et des transactions signés. En tant que moyen de relier le **proposant** et le **répondant** , le TSWAP est un élément central de l'écosystème TDEX. Tirant parti des protocoles de message et de transport susmentionnés, TSWAP comprend principalement quatre sous-éléments :

- **SwapRequest :** **&nbsp;****le proposant** initie l'échange.
- **SwapAccept :** le répondant accepte la demande.
- **SwapComplete :** le proposant confirme la connexion sécurisée.
- **SwapFail :** l'une ou l'autre des parties annonce la résiliation de l'échange en cas d'échec. À l'avenir, un élément supplémentaire - _failure_code - _ pourrait être implémenté pour indiquer la raison de l'échec.

#### 3.1.4 Protocole de négociation : BOTD # 4

Sans doute la mise en œuvre la plus cruciale pour TDEX, le protocole de négociation combine tous les BOTD précédents pour définir l'interface publique pour l'échange sans dépositaire. Contrairement au modèle de carnet d'ordres des échanges de dépôt, ce protocole permet aux *traders* et aux *teneurs de marché* de se connecter directement à l'aide de swaps atomiques.

Nous aborderons plus loin la question de l'écosystème pour les traders et les fournisseurs de liquidités. Pour l'instant, il devrait suffire de mentionner que les teneurs de marché représentent des démons *toujours actifs* et fournissent une liquidité proportionnelle aux paires d'actifs **Base-Quote**. À l'avenir, TDEX adoptera des contrats basés sur [Simplicity](https://blockstream.com/simplicity.pdf) pour renforcer encore la sécurité et la confidentialité de la plateforme, tout en permettant des fonctionnalités plus étendues.

### 3.2 TDEX pour les teneurs de marché

Sur le réseau TDEX, les *teneurs de marché* sont de telles entités qui fournissent des liquidités aux paires d'actifs à négocier en bourse, et peuvent donc également être appelées *fournisseurs de liquidités* (**fournisseur**). La fonction principale du fournisseur est de contenir une paire mutuellement indexée d'un actif de cotation (quote_asset) et d'un actif de base (base_asset). Il faut noter, cependant, que cela s'applique à n'importe quelle paire d'actifs et pas nécessairement à celles liées au Bitcoin.

Comme solution au problème classique de la [*double coïncidence des besoins*](https://www.oxfordreference.com/view/10.1093/oi/authority.20110803095622703), TDEX permet aux teneurs de marché d'exécuter des points d'extrémité *toujours actifs*, tout en révélant son adresse publique en utilisant l'un ou l'autre des canaux définis dans le BOTD #2. Cela garantit des marchés facilement accessibles aux traders, ce qui permet de remédier à l'un des principaux problèmes des échanges décentralisés.

#### 3.2.1 Implémentation du démon

Pour participer en tant que fournisseur, il faut implémenter un démon sur le réseau en l'exécutant via Docker ou en tant qu'entité autonome (En savoir plus: [Procédure d'implémentation du démon](https://docs.tdex.network/tdex-daemon.html) ). Un démon standard sur TDEX expose deux points de terminaison HTTP / 2 gRPC : l'**interface Trader** (publique) et l'**interface opérateur** (privée). Alors que l'interface publique représente le port pour les traders (par défaut : 9945), l'interface privée (par défaut : 9000) est utilisée pour les transactions internes du teneur de marché. En outre, pour une sécurité optimale, chaque démon dispose d'un [Blockstream Green](https://help.blockstream.com/hc/en-us/categories/900000056183-Blockstream-Green) ou Liquid Wallet pré-intégré.

#### 3.2.2 Stratégies de tenue de marché

L'un des éléments de différenciation de TDEX est qu'il offre de multiples options de tenue de marché aux fournisseurs, élargissant ainsi considérablement leur champ d'action. En d'autres termes, TDEX laisse les teneurs de marché choisir ou créer leurs stratégies, plutôt que d'imposer l'un ou l'autre.

Par défaut, le protocole adopte une stratégie CFMM (*Constant Function Market-Making*) pour déterminer les prix des actifs. Cependant, les teneurs de marché ont également la possibilité de mettre en œuvre des flux de prix (externes) *enfichables* à l'aide d'une API personnalisée. Considérant que l'implication des entreprises serait essentielle au succès de TDEX, les stratégies de tenue de marché personnalisées font partie des fonctionnalités les plus cruciales de la plateforme, en particulier parce qu'elle soutient simultanément la logique du choix des utilisateurs. En d'autres termes, alors que les fournisseurs ont le choix de sélectionner leur stratégie de prix, les traders souverains de la plateforme ont la capacité de choisir ou de rejeter ces stratégies.

#### 3.2.3 Frais de transaction

Alors que le ratio de réserve *base_asset-quote_asset* change avec chaque transaction, TDEX assure la cohérence de la taille globale du marché en prélevant des frais de transaction minimaux sur chaque transaction et en l'ajoutant aux réserves. Étant donné que l'arbitrage doit motiver un flux transactionnel cohérent, dans les cas où le teneur de marché met en œuvre une stratégie basée sur l'AMM, les revenus générés par les frais devraient augmenter avec le temps.

Parallèlement, cependant, TDEX adopte le [mécanisme](https://en.bitcoin.it/wiki/PayJoin) [P2EP](https://en.bitcoin.it/wiki/PayJoin), minimisant ainsi l'espace blockchain requis par les transactions, ce qui optimise efficacement les frais impliqués. Ceci est fait pour assurer un terrain de jeu équitable et de juste pour les commerçants et les fournisseurs sur la plateforme.

#### 3.2.4 Pools de liquidité (mise en œuvre future)

Plus tard sur sa feuille de route prévue, TDEX implémenterait une fonctionnalité *non-dépositaire* qui peut servir de cadre pour que les démons se connectent et mettent en commun leurs actifs. Une fois atteint, cela garantirait une liquidité plus grande et plus cohérente sur la plateforme, et exposerait un seul point final pour la commodité des traders. À son tour, TDEX sera en mesure de répondre aux demandes financières à grande échelle.

En tant que tel, le fournisseur qui crée un pool sera le *maître du pool* et d'autres fournisseurs pourront rejoindre le {em1maillage distribué du service pour agréger les liquidités. À titre d'incitation, le maître du pool sera investi de la capacité de déterminer le prix de base des actifs du pool et les opérateurs devront consulter les prix au comptant agrégés du fournisseur. Pour un actif donné, un fournisseur peut soit se présenter seul, soit rejoindre un pool, mais il ne peut pas assumer les deux positions simultanément.

### 3.3 TDEX pour les traders

Dans le contexte de TDEX, le *marché* est n'importe quelle paire d'actifs de base et de cotation qui peuvent être échangés de manière atomique. Comme mentionné sous BOTD # 3, un **Proposant** doit initier des swaps sur TDEX et, en variante, représenter un Trader sur le réseau. En d'autres termes, un trader sur TDEX est tout utilisateur qui implémente pleinement le protocole de négociation (BOTD # 4). Ce faisant, il se connecte à l'interface Trader précédemment discutée - le port public du démon du fournisseur - et accepte de négocier au taux de marché stipulé.

En général, le trading sur TDEX est similaire à tout autre échange basé sur un swap atomique, ce qui signifie que le trader peut échanger des proportions égales (par valeur marchande) des deux actifs de la paire. Cependant, contrairement à la majorité de ses pairs d'autres réseaux, le cadre de TDEX garantit la confidentialité, des règlements plus rapides et un glissement minimal ou nul. De plus, étant non dépositaire, TDEX soulage le trader des préoccupations concernant la perte de fonds en raison de piratages et de fuites.

#### 3.3.1 Kits de développement logiciel : la contribution open-source de TDEX pour LiFi

Outre l'interface utilisateur par défaut, la plateforme permet également aux traders de déployer leur client personnalisé à l'aide des kits de développement logiciel (SDK) de TDEX. Dans la phase initiale, cela peut être fait en utilisant [JavaScript](https://docs.tdex.network/tdex-sdk.html), mais à l'avenir, TDEX aura des SDK pour Python, Go et Rust. D'autre part, dans la phase initiale, les traders interagissent avec les fournisseurs à l'aide de l'[interface de ligne de commande](https://docs.tdex.network/tdex-cli.html#install) (CLI), jusqu'à ce que le futur plan d'une application mobile décentralisée se concrétise.

Ces SDK représentent essentiellent les contributions de TDEX aux capacités open-source du réseau, principalement en facilitant le travail des développeurs expérimentés dans l'implémentation d'API Bitcoin et d'autres fonctionnalités similaires. À cet égard, la vision plus large est de conduire des innovations au sein de l'écosystème Liquid, notamment dans le but de renforcer la génération de liquidité sur le réseau.

### 3.4 Cas d'utilisation

Après avoir parlé des divers éléments de l'écosystème TDEX, examinons maintenant certains des cas d'utilisation les plus importants et possibles.

#### 3.4.1 Marché secondaire pour les actifs liquides

Il faut en général garder à l'esprit que les actifs négociés sur le réseau TDEX sont essentiellement des actifs liquides. Ainsi, être un marché secondaire pour les L-Assets fait partie des principaux cas d'utilisation de la plat-forme TDEX, au moins dans les premières étapes.

En bref, Liquid permet à ses utilisateurs d '« émettre » des actifs transférables, allant de différentes classes d'actifs - fiat tokenisé et autres cryptomonnaies non-BTC, jetons non fongibles (objets de collection), jetons d'incitation (récompenses), marchandises tokenisées (par exemple, pièces d'or), et ainsi de suite. Chaque L-Asset a un identifiant de 64 caractères, qui peut être attaché à des domaines lisibles par l'homme sur la blockchain en publiant leurs métadonnées sur le « Registre des actifs » sur Blockstream.info, c'est-à-dire sur la version Liquid d'un Block Explorer. Le protocole permet également la réémission de jetons et les brûlures de jetons. Dans le contexte de TDEX, cela signifie que les fournisseurs peuvent créer des marchés pour n'importe quelle paire de L-Assests, facilitant ainsi les transactions sur ces actifs. De même, il pourrait être utilisé pour les transactions et les ventes NFT.

Il est cependant impératif de noter à ce stade un aspect crucial de la vision de TDEX : TDEX ne doit pas avoir de jeton natif, principalement parce que le projet est axé sur la communauté et ne donne pas la priorité à des motivations lucratives.

#### 3.4.2 Trading institutionnel et transfert de fonds

Les traders et les teneurs de marché du réseau TDEX ne doivent pas nécessairement être des particuliers, mais peuvent également être des institutions et des entreprises. Ainsi, la plateforme fournit un canal sécurisé pour une telle organisation pour échanger des L-Assets, qui à leur tour devraient jouer un rôle déterminant dans l'amélioration des adoptions à long terme et dans l'extension de la communauté.

Parallèlement, la boîte à outils open source de TDEX élargit encore la portée en offrant la possibilité aux entreprises, petites, moyennes et grandes, de déployer des solutions personnalisées pour répondre à leurs besoins financiers de manière décentralisée. En fait, c'est dans ce sens que l'objectif de TDEX de devenir un « réseau capital » pour LiFi peut être réalisé

## 4. Conclusion

Les problèmes de confidentialité et de sécurité se multiplient. Les obligations de conformité paralysent les échanges centralisés de plusieurs manières, tandis que les décentralisés compromettent la sécurité et tombent en proie à des piratages, des escroqueries et des fuites de plusieurs types. En fin de compte, sous l'effet combiné de ces facteurs, les utilisateurs perdent leur argent ou leurs données et, plus important encore, sont privés de leurs droits fondamentaux à la vie privée et à l'autonomie.

Développé dans ce contexte, TDEX est une solution décentralisée et axée sur la confidentialité déployée sur le réseau Liquid. Principalement un protocole de trading basé sur l'échange atomique, la plateforme dispose également d'une boîte à outils open source que les développeurs peuvent utiliser pour déployer des API personnalisées et d'autres solutions sur le réseau. Dans son ensemble, TDEX envisage de devenir un protocole de base facilitant les solutions décentralisées sur le réseau liquide, et à son tour, de renforcer les fondations de Liquid Finance (LiFi) en tant qu'espace sécurisé, sûr et méritocratique pour une communauté mondiale d'utilisateurs et de passionnés de crypto.

## Remerciements

Au moment de s'embarquer dans un voyage vers la construction de l'avenir, TDEX a été inspiré, conseillé et assisté par plusieurs personnes et entreprises. Conscients que le projet ne serait jamais possible sans eux, nous souhaitons saluer certaines des nombreuses contributions.

[Blockstream](https://blockstream.com/)

[Vulpem Ventures](https://vulpem.com/)

[Mohammad Musharraf](http://mohammadmusharraf.com/)

[Shiladitya Sinha](https://www.linkedin.com/in/shiladityasinhaofficial/)
