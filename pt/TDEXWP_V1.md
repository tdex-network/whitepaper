# TDEX: uma visão descentralizada para alavancar swaps atômicos para Trustless Finance

**White paper TDEX | Versão 1.1. | Junho de 2022**

**Resumo:** T(True) DEX é o primeiro projeto de troca atômica com prioridade em privacidade (DEX) desenvolvida na Liquid Network. Como um projeto de código-fonte aberto voltado para a comunidade, tem como objetivo de se tornar o framework para um ciberespaço rápido e seguro para usuários de Bitcoin, bem como um mercado secundário para Liquid Assets. Ao fazer isso, a TDEX facilita a geração de liquidez de uma forma que aproveita a segurança do Bitcoin, mas mitiga substancialmente suas deficiências de privacidade e fungibilidade, fortalecendo assim a base para Trustless Finance. Neste white paper, elaboramos o ecossistema do projeto e a visão subjacente que brilha como uma luz guia.

## 1. Introdução

As inovações tecnológicas são essenciais para o progresso humano e, na maioria das vezes, salvam e tornam nossas vidas melhores. Considerando seu imenso significado, a tecnologia deve ser idealmente acessível a todos, de forma igual e adequada. No entanto, esse não tem sido o caso.

Com foco no setor financeiro, não se pode negar que as inovações em FinTech melhoraram substancialmente a experiência geral do usuário final: pagamentos com um toque, cadernetas digitais, e-KYC e assim por diante. No entanto, embora a facilidade de uso adquirida supostamente impulsione um uso mais amplo, na realidade, os sistemas financeiros tradicionais têm estruturalmente excluído uma população global sem banco de cerca de [1.7 bilhões](https://globalfindex.worldbank.org/chapters/unbanked) de adultos.

A privacidade, por outro lado, foi drasticamente violada. Instituições governamentais e corporações com fins lucrativos não apenas se intrometem nas atividades online do usuário, mas também fazem uso indevido de seus dados pessoais para monitorar, censurar e anunciar. Indiscutivelmente, isso equivale a uma violação de um direito muito básico do usuário.

Primeiramente, este é um resultado direto do envolvimento de vários intermediários, como bancos, governos, agentes, corretores e assim por diante. Esses intermediários atuam como supervisores ou "confiança" e, no processo, surgem como pontos centrais de controle.

### 1.1 Bitcoin: Combinando Tecnologia Orientada ao Usuário

Em 2008, Satoshi Nakamoto lançou o Bitcoin [white paper](https://nakamotoinstitute.org/bitcoin/), apresentando uma combinação de quatro tecnologias potentes *orientadas ao usuário*, blockchain, criptografia, prova de trabalho e um sistema peer-to-peer no sentido de que eles restabelecem o controle pelos usuários, em vez por entidades governantes centralizadas. A inovação facilitou um novo paradigma econômico para transações monetárias ponto a ponto seguras dentro de um ecossistema distribuído e totalmente descentralizado. Ao enfrentar o problema do gasto duplo sem usar o modelo baseado em confiança, Satoshi eliminou efetivamente os intermediários do processo e os substituiu por um algoritmo computadorizado.

No entanto, apesar de ter todas as características de um bom dinheiro e reserva de valor, o Bitcoin, em sua forma esquelética, fica aquém de sua promessa de privacidade e fungibilidade. Em outras palavras, as transações de Bitcoin são pseudônimas e não anônimas, enquanto sua fungibilidade é desafiada pela análise de cadeia e assim por diante. Além disso, para obter segurança e resiliência ideais, o núcleo do Bitcoin faz compromissos essenciais em escalabilidade, tornando-o ineficiente para várias soluções e funcionalidades baseadas em Bitcoin. Posteriormente no artigo, discutiremos como a Liquid sidechain aborda esses problemas com o Layer-1 do Bitcoin.

### 1.2 O problema de geração de valor consistente

Na última década, a comunidade ficou superlotada e quase saturada com ativos criptográficos. Respaldados por promessas revolucionárias, esses ativos se tornaram populares rapidamente. No entanto, dadas as perdas gigantescas devidas a golpes, hacks e projetos fracassados, deve-se examinar criticamente se a maioria desses esforços realmente contribui para o progresso de longo prazo da comunidade. Mais importante, como eles se saem em termos dos princípios básicos do domínio?

**Trocas de Custódia**. Para consistência com o propósito imediato do TDEX, vamos tomar o exemplo das trocas centralizadas que são atualmente o principal gateway para interagir com a maioria dos ativos criptográficos. Para cumprir as obrigações regulatórias e garantir a liquidez, a maioria das plataformas de câmbio têm custódia: elas retêm o controle sobre os fundos do usuário, bem como as chaves privadas de sua carteira hospedada em bolsa.

A maioria das trocas de custódia são proprietárias, gerenciadas e administradas por entidades singulares, enquanto os fundos e os dados são armazenados em servidores centralizados. Consequentemente, para negociar e realizar transações nessas trocas, os usuários precisam interagir com esses servidores em silos que representam um *ponto de falha único*, expondo-os a altos riscos de violação de segurança e privacidade, censura e perda de fundos.

**Trocas Descentralizadas**. Como alternativa às trocas de custódia, várias trocas descentralizadas têm surgido. Em geral, elas implementam protocolos algorítmicos de "market-making", conhecidos como *Automated Market Makers* ou AMMs, determinando preços por meio de métricas de oferta e demanda, sem interferência de terceiros. No entanto, elas trazem seu próprio conjunto de perigos, dos quais as preocupações com escalabilidade são as mais relevantes no contexto deste artigo.

Parcialmente por causa de seus blockchains subjacentes e também como uma desvantagem da implementação de contratos inteligentes, a maioria dos DEXs não é escalonável, resultando em taxas de transação muito altas em períodos de congestionamento de rede. Em sua forma atual, à medida que um DEX se torna mais popular, ele também se torna infinitamente mais caro. Além disso, bugs em contratos inteligentes surgiram como um perigo comum para a indústria, levando os usuários a sofrer perdas substanciais com hacks e violações.

### 1.3 O projeto TDEX

Iniciado pela SevenLabs, o TDEX é um intercâmbio descentralizado baseado em Elementos, voltado para a comunidade e construído na Liquid Network. Aproveitando a segurança, usabilidade e velocidade combinadas da estrutura Bitcoin-Liquid, a TDEX prevê uma experiência de negociação rápida, segura e verdadeiramente descentralizada em Liquid Assets (L-Assets).

O protocolo TSWAP subjacente implementa trocas atômicas e resolve o problema de liquidez por meio de vários métodos de incentivos. A TDEX também capacita os provedores de liquidez, permitindo-lhes escolher sua estratégia de market-making. Por outro lado, os comerciantes ganham com taxas competitivas, liquidações mais rápidas, menor slippage e melhor segurança.

Nas seções a seguir, discutiremos os elementos de plano de fundo e primeiro plano do projeto TDEX. No processo, destacamos como o protocolo pode emergir como uma rede de backbone para Trustless Finance, permitindo que comerciantes profissionais e proprietários de negócios gerenciem, façam transações e invistam em um ambiente com prioridade para a privacidade.

## 2. O framework: segurança, privacidade e velocidade

Aproveitando um núcleo baseado em Elements, o TDEX é implantado na Liquid Network. Como uma sidechain do Bitcoin, o Liquid herda e aumenta sua segurança, enquanto melhora os aspectos de privacidade, fungibilidade e escalabilidade. Neste segmento, elucidamos a razão para adotar a Liquid como framework para TDEX.

Para resolver efetivamente as crises mencionadas de negociação descentralizada, a TDEX prevê uma solução holística e dupla. Por um lado, deve resolver algumas das preocupações primitivas da comunidade, como latência, privacidade inadequada e as ameaças à fungibilidade. Por outro lado, deve alargar o horizonte de soluções financeiras abertas, permitindo funcionalidades mais recentes em comparação com o núcleo do Bitcoin. Em outras palavras, a TDEX pretende diversificar a finalidade da camada 1 do Bitcoin e é precisamente neste ponto que sua visão se coaduna com a da Liquid, uma cadeia lateral de bitcoin da segunda camada.

Como os autores do Liquid [white paper](https://blockstream.com/assets/downloads/pdf/liquid-whitepaper.pdf) corretamente apontam, para o mundo de alta velocidade dos traders de criptomoedas, taxas de transação, a variação nos tempos de liquidação, as transações de transmissão pública, bem como os riscos de reorganizações da cadeia podem incorrer em custos significativos durante suas atividades comerciais.

Além do consenso Tolerante a Falhas Bizantinas (BFT) da rede que discutiremos brevemente, implementações como Transações Confidenciais e Emissão de Ativos pareceram ser as mais relevantes para o propósito da TDEX.

### 2.1 A Federação Forte &amp; Consenso BFT da Liquid

Para simplificar, a Liquid funciona com um mecanismo peg-in e peg-out, protegido por um conjunto *global e culturalmente distribuído* de "funcionários" formando coletivamente uma "[Federação Forte](https://blockstream.com/strong-federations.pdf)" de validadores. Para garantir que esses funcionários tenham sua *pele no jogo*, o protocolo exige que eles sejam bolsas, corretores e assim por diante ou seja, entidades com motivação substancial para garantir a estabilidade e o progresso da rede Bitcoin. A federação assina blocos, transações e *pegs* na Liquid usando módulos-chave que reforçam a lógica algorítmica para restringir bifurcações e transações não autorizadas. Além disso, o consenso BFT subjacente implementa um *round-robin, esquema de commit trifásico* e os blocos são assinados a cada minuto, sem envolver o risco de reorganização da cadeia.

Ao contrário da *distribuição de Poisson aleatória* do consenso de PoW do Bitcoin, o peg bidirecional federado da Liquid implica em várias melhorias na latência transacional. Por sua vez, isso permitiria a negociação e liquidação de transações quase em tempo real (~2 minutos) na rede TDEX, preservando a descentralização do protocolo, uma vez que a federação é um conjunto de participantes mutuamente não confiáveis. Além disso, o Liquid adota um vetor de limiar, onde *n* é o número total de funcionários e *k* representa o número mínimo de assinaturas necessárias para que um bloco seja considerado válido. Apesar da lacuna de que cada funcionário deve ter um relógio sincronizado adequadamente, o referido vetor permite que a rede alcance *segurança* e *vivência*, o que acaba se traduzindo em maior segurança e tempo de atividade para TDEX.

### 2.2 Transações confidenciais

No processo de desenvolvimento do TDEX, a compreensão de que a privacidade é um direito humano fundamental se apresentou como o substrato para a maioria das escolhas. O livro-razão público do Bitcoin registra todas as transações sem vinculá-las diretamente ao remetente e, aparentemente, isso é suficiente para a privacidade. No entanto, um olhar mais atento revela que *pseudonimato*, em uma extensão considerável, fica aquém de garantir *autonomia* para o usuário. Por exemplo, a *análise da cadeia* e o rastreamento do histórico de transações relacionado a uma determinada chave pública podem negar efetivamente o pseudonimato do usuário. Além disso, os padrões revelados no processo também podem ser usados para classificar moedas *boas* e *ruins*, o que é uma ameaça à *fungibilidade*. Atualmente, estão sendo desenvolvidas soluções para resolver esses problemas, que incluem a implementação do TDEX.

É preciso observar que a privacidade não se trata apenas de *segredo* em vez disso, ela implica que o usuário controla *se e quando* revelar uma determinada informação sobre si mesmo. Nesse sentido, a Liquid aprimora as métricas de privacidade do Bitcoin e, portanto, novamente, seu caminho se cruza com a jornada da TDEX.

Implementando componentes como *compromissos homomórficos*, *troca de chave Diffie-Hellman* e *range proofs*, entre outros, a Liquid permite [Transações Confidenciais](https://blockstream.com/bitcoin17-final41.pdf) em que tanto o montante quanto o tipo de ativo são ocultados. Em outras palavras, o valor e o tipo do ativo que está sendo transacionado são criptografados de tal forma que não podem ser descriptografados (abertos) com outro valor, nem podem ser determinados pelo compromisso. Presumindo o modelo *Unspent Transaction Output* (UTXO), este método prova a validade de uma transação ao demonstrar que <em>** entrada total = saída total **</em>, o que significa que não houve inflação, destruição ou gasto duplo no processamento. Além disso, a rede aproveita o *Asset Surjection Proof* (ASP) - uma forma de Zero-Knowledge Proofs em que o *asset tag* prova que está comprometido com um *recurso gasto*, mas não revela qual.

Como uma engrenagem principal no mecanismo da Liquid, as transações confidenciais adotam criptografias assimétricas usando *blinding keys*, ou seja, um par de chaves públicas e privadas. Entre outros resultados, ela minimiza os riscos de interceptação durante o processo de troca de chaves, tornando as transações idealmente privadas e resistentes à censura. Em termos simples, o processo pode ser resumido da seguinte forma:

- O proprietário do ativo, digamos Alice, transmite o endereço público da transação pretendida (swap). Compreensivelmente, isso é visível para toda a rede.
- Um receptor interessado, digamos Bob, *codifica sua chave pública cega* em um endereço que ele compartilha com Alice. No caso do TSWAP, essa troca ocorre por meio de um protocolo de mensagens criptografadas que, além de garantir a segurança, também permite que ambas as partes verifiquem os UTXOs envolvidos na transação.
- Ao receber a mensagem, Alice cria a transação e a criptografa com o endereço público de Bob. Bob (o receptor) é a única pessoa com a chave privada associada para essa transação e, portanto, apenas ele pode descriptografar a transação depois de gravada no blockchain. Nem mesmo Alice pode fazer isto.

Consequentemente, a rede atende a tais necessidades transacionais onde uma cobertura de transparência é bastante indesejável. Por exemplo, as transações confidenciais permitem que as empresas conduzam os processos financeiros de forma descentralizada e verificável, mas simultaneamente protegem as informações confidenciais da exposição ao público. Da mesma forma, o princípio fortalece o ímpeto para a adoção de Bitcoin em outros setores relevantes, como finanças governamentais e assim por diante.

## 3. O ecossistema TDEX

O surgimento de soluções descentralizadas da Liquid Network - ou, como Adam Back, o CEO da Blockstream, a chama, Liquid Finance ou LiFi - tem ganhado força substancial recentemente. Consequentemente, uma quantidade cada vez maior de valor está sendo gerada na rede, especialmente na forma de Ativos Líquidos. Por sua vez, a TDEX se esforça para atender à crescente demanda da comunidade por um mercado secundário descentralizado para esses ativos, além de ser um kit de ferramentas de código aberto para promover mais inovação.

Nas seções anteriores, discutimos a estrutura da TDEX e as razões por trás de algumas de suas escolhas cruciais. Agora, elaboramos o ecossistema do protocolo, apresentando ao leitor uma visão geral dos protocolos e implementações.

### 3.1 Os pilares técnicos: Noções básicas de True DEX (BOTD)

No núcleo do TDEX, existem quatro protocolos *Mensagem*, *Transporte, Swap* e *Trade*, que discutiremos neste segmento. No entanto, a este respeito, o artigo abstém-se deliberadamente de elaborar as exposições técnicas completas que estão disponíveis nas documentações técnicas em [Especificações TDEX](https://dev.tdex.network/docs/specs/index).

#### 3.1.1 Protocolo de Mensagem: BOTD #1

Um requisito fundamental, primitivo, para a rede descentralizada da TDEX é um canal de mensagens bidirecional seguro para conectar contrapartes. Essa conexão deve ser confiável, estável, ponto a ponto (P2P) e, acima de tudo, com prioridade para a privacidade. Aproveitando a Liquid, a TDEX pode atender a esses requisitos para *comunicações confidenciais*. Além disso, para serializar essas mensagens, a TDEX implementa o *Protocol Buffers* do Google - um método independente de plataforma e linguagem para serializar dados estruturados.

#### 3.1.2 Protocolo de Transporte: BOTD #2

Para realizar transações na rede, os daemons (usuários) requerem canais de transporte P2P, em que a necessidade de confidencialidade e segurança se aplica de forma semelhante ao protocolo de mensagem. A este respeito, o TDEX fornece várias opções com um grau variável de privacidade que o usuário pode implementar isoladamente ou em combinação — *Texto claro* (inseguro), *Serviço Onion* (onion), *TLS do lado do servidor* (TLS), *TLS Mútuo* (mTLS ) e _Noise \ _XK \ _secp256k1 \ _ChaChaPoly \ *SHA256* (noise). Ao participar da rede TDEX, os usuários devem declarar seu canal de transporte implementado.

#### 3.1.3 Protocolo de Swap: BOTD #3

O protocolo TSWAP é uma implementação segura baseada em trocas atômicas que permite que os pares na rede troquem mensagens e transações assinadas. Como meio de fazer a ponte entre o **Proponente** e o **Respondente**, o TSWAP é um elemento central do ecossistema TDEX. Aproveitando a mensagem mencionada e os protocolos de transporte, o TSWAP tem quatro subelementos principais:

- **SwapRequest:** O proponente inicia a troca.
- **SwapAccept:** o respondente aceita a solicitação.
- **SwapComplete:** o proponente confirma a conexão segura.
- **SwapFail:** qualquer uma das partes anuncia o encerramento da troca em caso de falha. No futuro, um elemento adicional - _failure_code - _pode ser implementado para denotar o motivo da falha.

#### 3.1.4 Protocolo de Trade: BOTD #4

Indiscutivelmente a implementação mais crucial para o TDEX, o Protocolo de Trade combina todos os BOTDs anteriores para definir a interface pública para trocas não custodiais. Ao contrário do modelo de livro de pedidos de trocas de custódia, este protocolo permite que *traders* e *market makers* se conectem diretamente usando swaps atômicos.

Em uma seção posterior, discutiremos o ecossistema para usuários e provedores de liquidez. Atualmente, deve ser suficiente mencionar que os formadores de mercado representam *sempre-on* daemons e fornecem liquidez proporcional aos pares de ativos **Base-Quote**. No futuro, a TDEX adotaria contratos baseados em <a>Simplicidade</a> para aprimorar ainda mais a segurança e privacidade da plataforma, ao mesmo tempo em que possibilita funcionalidades mais amplas.

### 3.2 TDEX para Market Makers #2

Na rede TDEX, *Market Makers* são entidades que fornecem liquidez aos pares de ativos a serem negociados na bolsa e, portanto, também podem ser chamados de *Liquidity Providers* (** Provider **). A principal função do Provider é manter um par vinculado mutuamente de um Ativo de Cotação (quote_asset) e um Ativo de Base (base _asset). Deve-se notar, no entanto, que isso se aplica a qualquer par de ativos e não necessariamente aos indexados a Bitcoin.

Como uma solução para o problema clássico de [*Dupla Coincidência de Desejo*](https://www.oxfordreference.com/view/10.1093/oi/authority.20110803095622703), o TDEX permite que os market makers executem pontos finais *always-on*, ao mesmo tempo que revelam seu endereço acessível publicamente usando um dos canais definidos no BOTD # 2. Isto garante mercados prontamente disponíveis para os traders, abordando assim um dos principais problemas das bolsas descentralizadas.

#### 3.2.1 Implementação do Daemon #3

Para participar como Provider, é necessário implementar um Daemon na rede executando-o através do Docker ou como uma entidade autônoma (Leia mais: [Procedimento de implementação do Daemon](https://docs.tdex.network/tdex-daemon.html). Um daemon padrão no TDEX expõe dois endpoints HTTP/2 gRPC - a **Trader Interface** (pública) e a **Operator Interface** (privada). Enquanto a interface pública representa a porta para comerciantes (padrão: 9945), a interface privada (padrão: 9000) é usada para as transações internas do market maker. Além disso, para segurança ideal, cada daemon tem um <a>Blockstream Green</a> pré-incorporado ou um Liquid Wallet.

#### 3.2.2 Estratégias de market maker

Um dos elementos de diferenciação da TDEX é que ela fornece múltiplas opções de market-making para Providers, ampliando significativamente seu escopo. Em outras palavras, a TDEX permite que os market makers escolham ou criem suas estratégias, ao invés de impor uma ou outra.

Por padrão, o protocolo adota uma estratégia *Constant Function Market-Making* (CFMM) para determinar os preços dos ativos. No entanto, os market-makers também têm a opção de implementar feeds de preços *pluggable* (externos) usando uma API personalizada. Considerando que o envolvimento dos negócios seria fundamental para o sucesso da TDEX, as estratégias de market-making personalizadas estão entre as funcionalidades mais cruciais da plataforma, especialmente porque simultaneamente mantém a lógica que os usuários escolham. Em outras palavras, enquanto os Providers têm a opção de selecionar sua estratégia de preços, os traders soberanos da plataforma têm a capacidade de escolher ou rejeitar essas estratégias.

#### 3.2.3 Taxa de swap

Enquanto a taxa de reserva *base_asset-quote_asset* muda com cada negociação, a TDEX garante consistência no tamanho geral do mercado cobrando uma taxa de swap mínima em cada negociação e adicionando-a às reservas. Considerando que a arbitragem deve motivar um fluxo transacional consistente, nos casos em que o market maker implemente uma estratégia baseada em AMM, a receita gerada com a taxa deve aumentar ao longo do tempo.

Paralelamente, no entanto, o TDEX adota o mecanismo [P2EP](https://en.bitcoin.it/wiki/PayJoin), minimizando assim o espaço de blockchain necessário por transações que efetivamente otimizam a taxa envolvida. Isso é feito para garantir um playground justo e nivelado para Traders e Providers no protocolo.

#### 3.2.4 Pools de liquidez (implementação futura)

Mais adiante em seu roteiro pretendido, o TDEX implementaria uma funcionalidade *non-custodial* que pode atuar como o framework para que os daemons se conectem e agrupem seus ativos. Uma vez alcançado, isto garantiria uma liquidez maior e mais consistente no protocolo, bem como exporia um único ponto de extremidade para a conveniência dos usuários. Por sua vez, a TDEX será capaz de acomodar demandas financeiras em escala.

Como tal, o Provider que cria um pool será o *Pool Master* e outros provedores poderão se juntar à *distributed service mesh* para agregar liquidez. Como um incentivo, o mestre do pool será investido com a capacidade de determinar o preço base para os ativos do pool e os negociadores terão que consultar os preços à vista agregados do fornecedor. Para qualquer ativo, um provedor pode operar sozinho ou ingressar em um pool, mas não pode assumir as duas posições simultaneamente.

### 3.3 TDEX para comerciantes

No contexto do TDEX, o *mercado* é qualquer par de ativos de base e de cotação que podem ser trocados de forma atômica. Conforme mencionado no BOTD #3, um **Proponente** deve iniciar trocas no TDEX e, alternativamente, representar um Trader na rede. Em outras palavras, um Trader em TDEX é qualquer usuário que implementa totalmente o Protocolo de Trade (BOTD# 4). Ao fazer isso, ele se conecta com a Trader Interface discutida anteriormente - a porta pública do daemon do Provider - e concorda em negociar na taxa de mercado estipulada.

Em geral, a negociação na TDEX é semelhante a qualquer outra bolsa baseada em swap atômico, o que significa que o negociante pode trocar proporções iguais (por valor de mercado) de ambos os ativos do par. No entanto, ao contrário da maioria de seus pares de outras redes, a estrutura da TDEX garante a confidencialidade, liquidações mais rápidas e mínima ou nenhuma derrapagem. Além disso, por não ter custódia, o TDEX alivia o usuário de preocupações sobre a perda de fundos para hacks e violações.

#### 3.3.1 Kits de desenvolvimento de software: Contribuição de código aberto da TDEX para LiFi

Além da IU padrão, o protocolo também permite que os usuários implantem seus clientes personalizados usando os kits de desenvolvimento de software (SDK) da TDEX. Na fase inicial, isso pode ser feito usando [JavaScript](https://docs.tdex.network/tdex-sdk.html), mas no futuro, TDEX terá SDKs para Python, Go e Rust. Por outro lado, na fase inicial, os comerciantes interagem com os provedores usando a [Interface de linha de comando](https://docs.tdex.network/tdex-cli.html#install)(CLI), até que se concretize o futuro plano de um aplicativo descentralizado e móvel.

Essencialmente, esses SDKs representam as contribuições da TDEX para os recursos de código aberto da rede, principalmente ao capacitar desenvolvedores versados na implementação de API de bitcoin e outras funcionalidades semelhantes. Nesse sentido, a visão mais ampla é impulsionar inovações no ecossistema Liquid, principalmente com o objetivo de fortalecer a geração de liquidez na rede.

### 3.4 Casos de uso

Tendo discutido os vários elementos do ecossistema TDEX, vejamos agora alguns dos casos de uso proeminentes e possíveis.

#### 3.4.1 Mercado Secundário para Liquid Assets

Em geral, deve-se ter em mente que os ativos trocados na rede TDEX são essencialmente Liquid Assets. Assim, ser um mercado secundário para L-Assets está entre os principais casos de uso da plataforma TDEX, pelo menos nos estágios iniciais.

Resumidamente, o Liquid permite que seus usuários emitir ativos transferíveis, que variam entre as classes de ativos - fiat tokenizado e outras criptomoedas não BTC, tokens não fungíveis (itens colecionáveis), tokens de incentivo (recompensas), commodities tokenizadas (por exemplo, moedas de ouro) e assim por diante. Cada L-asset tem um identificador de 64 caracteres, que pode ser anexado a domínios legíveis por humanos no blockchain, publicando seus metadados no Asset Registry em Blockstream.info isto é, na versão do Liquid de um Block Explorer. O protocolo também permite tokens de reemissão e queima de token. No contexto da TDEX, isso significa que os Provedores podem criar mercados para qualquer par de L-ativos, facilitando assim as negociações desses ativos. Da mesma forma, pode ser aproveitado para transações e vendas NFT.

Neste ponto, no entanto, é imperativo observar um aspecto crucial da visão da TDEX - a TDEX não deve ter nenhum token nativo, principalmente porque o projeto é voltado para a comunidade e não prioriza quaisquer motivos lucrativos.

#### 3.4.2 Negociação institucional &amp; transferência de fundos

Usuários e Market Makers na rede TDEX não precisam ser necessariamente indivíduos, mas também podem ser instituições e empresas. Assim, a plataforma fornece um canal seguro para tal organização negociar com L-assets, que por sua vez, deve desempenhar um papel determinante no aumento das adoções de longo prazo e na ampliação da comunidade.

Paralelamente, o kit de ferramentas de código aberto da TDEX amplia ainda mais o escopo, estabelecendo a possibilidade de empresas pequenas, médias e grandes implantar soluções personalizadas para atender às suas necessidades financeiras de maneira descentralizada. Na verdade, é neste sentido que o objetivo da TDEX se tornar uma rede de backbone para Trustless Finance pode ser realizado.

## 4. Conclusão

As preocupações com privacidade e segurança estão crescendo rapidamente. As obrigações de conformidade estão paralisando as trocas centralizadas de várias maneiras, enquanto as descentralizadas estão comprometendo a segurança e sendo vítimas de hacks, golpes e violações de vários tipos. Em última análise, como um efeito combinado desses fatores, os usuários estão perdendo seu dinheiro ou seus dados e, mais importante, estão sendo privados de seus direitos básicos de privacidade e autonomia.

Desenvolvido com este pano de fundo, o TDEX é um protocolo descentralizado com prioridade para privacidade implantada na Liquid Network. Principalmente um protocolo de negociação baseado em swaps atômicos, a plataforma também tem um kit de ferramentas de código aberto que os desenvolvedores podem usar para implantar APIs personalizadas e outras soluções na rede. Como um todo, a TDEX prevê se tornar um protocolo de backbone facilitando soluções descentralizadas na Liquid Network e, por sua vez, fortalecendo a fundação da Trustless Finance como um espaço seguro, protegido e meritocrático para uma comunidade global de usuários Bitcoin e entusiastas.

## Agradecimentos

A caminho da construção do futuro, a TDEX foi inspirada, aconselhada e assistida por várias pessoas e empresas. Percebendo que o projeto nunca seria possível sem eles, gostaríamos de agradecer algumas das muitas contribuições.

[Blockstream](https://blockstream.com/)

[Vulpem Ventures](https://vulpem.com/)

[Mohammad Musharraf](http://mohammadmusharraf.com/)

[Shiladitya Sinha](https://www.linkedin.com/in/shiladityasinhaofficial/)

Acima de tudo, obrigado Satoshi Nakamoto
