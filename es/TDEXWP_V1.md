# TDEX: Una visión descentralizada para aprovechar los intercambios atómicos para Trustless Finance

**Libro blanco de TDEX | Versión 1.1 | Junio de 2022**

**Resumen:** T(True)DEX es la primera plataforma de cambio descentralizada (DEX) basada en intercambios atómicos y que prioriza la privacidad de su clase creada en Liquid Network. Como solución de código abierto orientada a la comunidad, su objetivo es convertirse en el sistema de un ciberespacio rápido y seguro para los usuarios de Bitcoin, así como un mercado secundario para los activos líquidos. Al hacerlo, TDEX facilita la generación de liquidez de forma que aprovecha la seguridad del Bitcoin, pero mitiga sustancialmente sus deficiencias de privacidad y fungibilidad, lo que refuerza el fundamento de Trustless Finance. En este libro blanco, explicamos el ecosistema del proyecto y la visión subyacente que brilla como un faro.

## 1. Introducción

Las innovaciones tecnológicas son fundamentales para el progreso humano y, a menudo, salvan y mejoran vidas. Teniendo en cuenta su inmensa importancia, la tecnología debería ser idealmente accesible para todos, por igual y de manera adecuada. Sin embargo, ese no ha sido el caso.

Centrándonos en el sector financiero, no se puede negar que las innovaciones en tecnología financiera han mejorado sustancialmente la experiencia general del usuario final: pagos con un solo toque, libretas digitales, conocimiento del cliente de manera electrónica (e-KYC), etc. Sin embargo, aunque la facilidad de uso adquirida supuestamente impulsa un uso más amplio, en realidad, los sistemas financieros tradicionales han excluido estructuralmente a una población mundial no bancarizada de alrededor de [1700 millones](https://globalfindex.worldbank.org/chapters/unbanked) de adultos.

La privacidad, por otro lado, se ha infringido drásticamente. Las instituciones gubernamentales y las corporaciones con ánimo de lucro no solo se entrometen en las actividades en línea del usuario, sino que además hacen un mal uso de sus datos personales para monitorizar, censurar y anunciar. Podría decirse que supone una infracción de un derecho muy básico del usuario.

Principalmente, esto es resultado directo de la participación de varios intermediarios como bancos, gobiernos, agentes, corredores, etc. Estos intermediarios actúan como supervisores o «fideicomisos» y, de paso, emergen como puntos centrales de control.

### 1.1 Bitcoin: Combinando tecnología orientada al usuario

En 2008, Satoshi Nakamoto publicó el [libro blanco](https://nakamotoinstitute.org/bitcoin/) del Bitcoin, que presenta una combinación de cuatro potentes tecnologías *orientadas al usuario:* cadena de bloques, criptografía, prueba de trabajo y entre iguales (P2P), en el sentido de que restablecen el control con los usuarios, en lugar de con entidades de gobierno centralizado. La innovación facilitó un nuevo paradigma económico para transacciones monetarias seguras entre iguales dentro de un ecosistema distribuido y completamente descentralizado. Al abordar el problema del doble gasto sin utilizar el modelo basado en la confianza, Satoshi eliminó de manera eficaz a los intermediarios terceros del proceso y los reemplazó con un algoritmo computarizado.

Sin embargo, a pesar de tener todas las características de una moneda fuerte y reserva de valor, el Bitcoin, en su base, no cumple su promesa de privacidad y fungibilidad. En otras palabras, las transacciones de Bitcoin son seudónimas y no anónimas, mientras que su fungibilidad se ve comprometida por el análisis de la cadena, etc. Además, para lograr una seguridad y resiliencia óptimas, el núcleo del Bitcoin hace concesiones esenciales en cuanto a escalabilidad, lo que lo vuelve ineficiente para varias soluciones y funcionalidades basadas en criptografía. Más adelante, veremos cómo la cadena lateral de Liquid aborda estos problemas con la Capa 1 del Bitcoin.

### 1.2 El problema de generar valor sistemático

Durante la última década, la comunidad se ha llenado y casi saturado de criptoactivos. Respaldados por promesas disruptivas, estos activos se han vuelto rápidamente muy populares. Sin embargo, dadas las enormes pérdidas atribuidas a estafas, piratas informáticos y proyectos fallidos, uno debe examinar críticamente si la mayoría de estas iniciativas realmente contribuyen al progreso de la comunidad a largo plazo. Y más importante aún, ¿cómo avanzan en relación con los principios fundamentales del dominio?

**Plataformas de cambio de custodia**. Por coherencia con el propósito inmediato de TDEX, tomemos el ejemplo de las plataformas centralizadas que actualmente son la puerta de enlace principal para interactuar con la mayoría de los criptoactivos. Para cumplir las obligaciones reglamentarias y garantizar la liquidez, la mayoría de las plataformas de cambio son de custodia: retienen el control sobre los fondos del usuario, así como las claves privadas de la billetera alojada en la plataforma.

La mayoría de las plataformas de custodia son propiedad de entidades singulares que las gestionan y gobiernan, mientras que los fondos y los datos se almacenan en servidores centralizados. En consecuencia, para realizar transacciones en estas plataformas, los usuarios deben interactuar con servidores aislados que representan un *punto único de fallo*, que los expone a riesgos elevados de infracción en la seguridad y privacidad, censura y pérdida de fondos.

**Plataformas descentralizadas**. Como alternativa a las plataformas de custodia, han proliferado varias plataformas descentralizadas. En general, implementan protocolos algorítmicos de creación de mercados, comúnmente conocidos como *Creadores de mercado automatizados* (AMM, por sus siglas en inglés), que determinan los precios a través de métricas de oferta y demanda, sin interferencia de terceros. Sin embargo, no están exentos de peligros, de los cuales la preocupación en materia de escalabilidad es el más relevante en el contexto de este documento.

En parte debido a sus cadenas de bloques subyacentes y también como desventaja a la hora de implementar contratos inteligentes, la mayoría de las DEX no son escalables, lo que da lugar a tarifas de transacción muy altas en períodos de congestión de la red. En su forma actual, a medida que una DEX se hace más popular, también se vuelve infinitamente más cara. Además, los errores en los contratos inteligentes han surgido como un peligro común para el sector, lo que lleva a los usuarios a sufrir notables pérdidas por ataques e infracciones.

### 1.3 El proyecto TDEX

Iniciada por SevenLabs, TDEX es una plataforma de cambio descentralizada basada en elementos y orientada a la comunidad creada en Liquid Network. Aprovechando la seguridad, usabilidad y velocidad combinadas del sistema Bitcoin-Liquid, TDEX prevé una experiencia rápida, segura y verdaderamente descentralizada en activos líquidos (L-Assets).

El protocolo TSWAP subyacente implementa intercambios atómicos y resuelve el problema de liquidez a través de varios incentivos «cero a uno». TDEX también empodera a los proveedores de liquidez al permitirles elegir su estrategia de creación de mercado. Por otro lado, los traders se benefician de tarifas competitivas, liquidaciones más rápidas, menor retraso y mejor seguridad.

En las secciones siguientes, hablamos de los elementos de primer y segundo plano del proyecto TDEX. De paso, destacamos cómo el protocolo podría surgir como una red troncal para Trustless Finance (LiFi), al permitir a traders profesionales y propietarios de empresas gestionar, realizar transacciones e invertir dentro de un entorno donde se prioriza la privacidad.

## 2. El sistema: seguridad, privacidad y velocidad

Al aprovechar un núcleo basado en elementos, TDEX se implementa en Liquid Network. Como cadena lateral del Bitcoin, Liquid hereda y mejora su seguridad, al tiempo que mejora los aspectos de privacidad, fungibilidad y escalabilidad. En este segmento, explicamos las razones de la adopción de Liquid como sistema para TDEX.

Para resolver eficazmente las crisis antes mencionadas del trading descentralizado, TDEX prevé una solución integral y doble. Por un lado, debe resolver algunas de las preocupaciones originales de la comunidad, como la latencia, la privacidad inadecuada y las amenazas a la fungibilidad. Por otro lado, debe ampliar el horizonte de las soluciones financieras abiertas, permitiendo funcionalidades más modernas en comparación con el núcleo del Bitcoin. En otras palabras, TDEX pretende diversificar el propósito de la capa 1 del Bitcoin y es precisamente en este punto donde su visión se compara con la de Liquid, una cadena lateral del Bitcoin de capa 2.

Como señalan acertadamente los autores del [libro blanco](https://blockstream.com/assets/downloads/pdf/liquid-whitepaper.pdf) de Liquid, *«para el mundo de alta velocidad del trader de criptomonedas, las tarifas de transacción, la variación en los tiempos de liquidación, las transacciones de transmisión pública, así como los riesgos de reorganizaciones de la cadena pueden incurrir en costes significativos durante sus actividades profesionales».*

Aparte del consenso de Tolerancia a faltas bizantinas (BFT, por sus siglas en inglés) de la red sobre el que hablaremos brevemente, implementaciones como transacciones confidenciales y emisión de activos parecían ser las más relevantes a efectos de TDEX.

### 2.1 Strong Federation y el consenso BFT de Liquid

En pocas palabras, Liquid funciona con un mecanismo de vinculación y desvinculación, protegido por un conjunto de «funcionarios» *distribuidos global y culturalmente*, que forman colectivamente una «[Strong Federation](https://blockstream.com/strong-federations.pdf)» (federación fuerte) de validadores. Para asegurar que estos funcionarios *participen en el juego*, el protocolo requiere que sean plataformas de cambio, intermediarios, etc., es decir, entidades con una motivación sustancial para garantizar la estabilidad y el progreso de la red Bitcoin. La federación firma bloques, transacciones y *vínculos* en Liquid utilizando «módulos clave» que fuerzan a la lógica algorítmica a restringir bifurcaciones y transacciones no autorizadas. Además, el consenso BFT subyacente implementa un *sistema de compromiso de tres fases y por turnos* y los bloques se firman cada minuto, sin implicar el riesgo de reorganización de la cadena.

A diferencia de la *distribución aleatoria de Poisson* del consenso de prueba de trabajo (PoW, por sus siglas en inglés) del Bitcoin, la vinculación bidireccional federada de Liquid implica múltiples mejoras en la latencia transaccional. A su vez, esto permitiría la liquidación de transacciones casi en tiempo real (~ 2 minutos) en la red TDEX, al tiempo que se preserva la descentralización del protocolo, ya que la federación es un conjunto de participantes sin confianza mutua. Además, Liquid adopta un vector de umbral, donde *n* es el número total de funcionarios y *k* representa el número mínimo de firmas necesarias para que un bloque se considere válido. A pesar del inconveniente de que todo funcionario debe tener un reloj adecuadamente sincronizado, dicho vector permite que la red alcance *seguridad* y *viveza* , lo que en última instancia se traducirá en una mayor seguridad y actividad para TDEX.

### 2.2 Transacciones confidenciales

En el proceso de desarrollo de TDEX, la constatación de que la privacidad es un derecho humano fundamental se planteó como el sustrato de la mayoría de las elecciones. El libro de registro público del Bitcoin registra todas las transacciones sin vincularlas directamente al remitente y, aparentemente, esto es suficiente para la privacidad. Sin embargo, una mirada más atenta revela que el *seudonimato*, en gran medida, no garantiza la *autonomía* del usuario. Por ejemplo, el *análisis de la cadena* y el seguimiento del historial de transacciones relacionado con una determinada clave pública podrían negar efectivamente el seudonimato del usuario. Además, los patrones revelados en el proceso también podrían usarse para clasificar las monedas en *buenas* y *malas*, lo cual es una amenaza para la *fungibilidad*. Actualmente, se están desarrollando soluciones para resolver estos problemas, que incluyen la implementación de TDEX.

Uno debe advertir que la privacidad no trata meramente sobre el *secreto*, sino más bien que el usuario controle *si y cuando* revelar un determinado dato suyo. En este aspecto, Liquid mejora las métricas de privacidad del Bitcoin, y por tanto, de nuevo, su camino se cruza en el viaje de TDEX.

Al implementar componentes como *compromisos homomórficos*, *intercambio de claves Diffie-Hellman* y *pruebas de rango*, entre otros, Liquid permite las «[Transacciones confidenciales](https://blockstream.com/bitcoin17-final41.pdf)», en las que se ciegan tanto el monto como el tipo de activo. En otras palabras, el monto y el tipo de activo objeto de la transacción se cifran de tal manera que no se pueden descifrar (abrir) con otro valor, ni se pueden determinar dado el compromiso. Teniendo en cuenta el modelo de *Resultado de transacciones no gastadas* (UTXO, por sus siglas en inglés), este método demuestra la validez de una transacción al probar que la _ **contribución total = resultado total** _, lo que significa que no ha habido inflación, destrucción o doble gasto en el proceso. Además, la red aprovecha la *Asset Surjection Proof* (ASP), un tipo de pruebas de conocimiento cero en las que, para resumir, la «*etiqueta del activo*» prueba que está comprometida con un *activo gastado*, pero no revela cuál.

Como engranaje principal en la máquina de Liquid, las transacciones confidenciales adoptan cifrados asimétricos que utilizan *claves cegadoras*, es decir, un par de claves pública y privada. Entre otros resultados, minimiza los riesgos de interceptación durante el proceso de intercambio de claves, lo que hace que las transacciones sean privadas de forma óptima y resistentes a la censura. En términos simples, el proceso se puede resumir de la siguiente manera:

- El propietario del activo (remitente), por ejemplo, Alice, transmite la dirección pública de la transacción prevista (intercambio). Lógicamente, esto sería visible en toda la red.
- Un receptor interesado, digamos Bob, *codifica su clave pública cegadora* en una dirección que comparte con Alice. En el caso de TSWAP, este intercambio se produce mediante un protocolo de mensajería cifrada que, además de garantizar la seguridad, también permite a ambas partes verificar los UTXO involucrados en la transacción.
- Al recibir el mensaje, Alice crea la transacción y la cifra con la dirección pública de Bob. Bob (el receptor) es la única persona con la clave privada asociada para esta transacción y, por lo tanto, solo él puede descifrar la transacción después de que se registre en la cadena de bloques, ni siquiera Alice.

En consecuencia, la red aborda tales necesidades transaccionales en las que una «transparencia» general resulta bastante indeseable. Por ejemplo, las transacciones confidenciales permiten a las empresas llevar a cabo procesos financieros de manera descentralizada y verificable, pero al mismo tiempo protege la información sensible de su exposición pública. De manera similar, este principio refuerza el ímpetu para la adopción del Bitcoin en otros sectores relevantes, como las finanzas gubernamentales, etc.

## 3. El ecosistema TDEX

La aparición de soluciones descentralizadas en Liquid Network, o, como lo llama Adam Back, CEO de Blockstream, Liquid Finance o LiFi, ha cobrado recientemente una fuerza sustancial. En consecuencia, se está generando una cantidad creciente de valor en la red, especialmente en forma de activos líquidos. A su vez, TDEX se esfuerza por abordar la creciente demanda de la comunidad de un mercado secundario descentralizado para estos activos, además de ser un conjunto de herramientas de código abierto para fomentar una mayor innovación.

En las secciones anteriores, hemos explicado el sistema de TDEX y las razones que hay detrás de algunas de sus elecciones cruciales. Ahora, explicaremos el ecosistema del protocolo, y presentaremos al lector una descripción general de los protocolos y las implementaciones.

### 3.1 Los pilares técnicos: conceptos básicos de True DEX (BOTD)

En el núcleo de TDEX, hay cuatro protocolos: *mensaje*, *transporte, intercambio* y *comercio*, que analizaremos en este segmento. Sin embargo, en este sentido, el documento se abstiene deliberadamente de elaborar exposiciones técnicas completas que están disponibles en la documentación técnica bajo [Especificaciones de TDEX](https://dev.tdex.network/docs/specs/index).

#### 3.1.1 Protocolo de mensajes: BOTD #1

Un requisito fundamental, llamado primitivo, para la red descentralizada de TDEX es un canal de mensajería bidireccional seguro para conectar a las contrapartes. Dicha conexión debe ser fiable, estable, entre iguales (P2P) y, sobre todo, que priorice la privacidad. Al utilizar Liquid, TDEX puede cumplir estos requisitos en las *comunicaciones confidenciales*. Además, para serializar estos mensajes, TDEX implementa los *búferes de protocolo* de Google, una plataforma y un método independiente del lenguaje para serializar datos estructurados.

#### 3.1.2 Protocolo de transporte: BOTD #2

Para realizar transacciones en la red, los daemons (usuarios) requieren canales de transporte P2P, en los que la necesidad de confidencialidad y seguridad se aplica de manera similar al protocolo de mensajes. En este sentido, TDEX ofrece varias opciones con un grado variable de privacidad que el usuario puede implementar de forma aislada o en combinación: *texto sin cifrar* (inseguro), *servicio Onion* (onion), *TLS del lado del servidor* (TLS), *TLS mutuo* (mTLS ) y *Noise_XK_secp256k1_ChaChaPoly_SHA256* (ruido). Mientras participan en la red TDEX, los usuarios deben declarar su canal de transporte implementado.

#### 3.1.3 Protocolo de intercambio: BOTD #3

El protocolo TSWAP es una implementación segura basada en intercambio atómico que permite a los pares en la red intercambiar mensajes y transacciones firmados. Como medio para tender un puente entre el **proponente** y el **respondedor**, TSWAP es un elemento fundamental del ecosistema TDEX. Al aprovechar los protocolos de mensajes y transporte antes mencionados, TSWAP tiene principalmente cuatro subelementos:

- **SwapRequest::** El **proponente** inicia el intercambio.
- **SwapAccept:** el respondedor acepta la solicitud.
- **SwapComplete:** el proponente confirma la conexión segura.
- **SwapFail:** cualquiera de las partes anuncia la finalización del intercambio al producirse un fallo. En el futuro, se podría implementar un elemento adicional (_failure_code) para indicar la razón del fallo.

#### 3.1.4 Protocolo comercial: BOTD #4

Posiblemente la implementación más crucial para TDEX, el protocolo comercial combina todos los BOTD anteriores para definir la interfaz pública para la plataforma sin custodia. Al contrario del modelo de libro de órdenes de las plataformas de custodia, este protocolo permite a *traders* y *creadores de mercado* conectarse directamente mediante intercambios atómicos.

En una sección posterior, analizaremos el ecosistema para usuarios y proveedores de liquidez. Actualmente, debería ser suficiente mencionar que los creadores de mercado representan daemons *siempre activos* y ofrecen liquidez proporcional a los pares de **Activo base y Activo cotizado**. En el futuro, TDEX adoptaría contratos basados sobre  [Simplicity](https://blockstream.com/simplicity.pdf) para mejorar aún más la seguridad y privacidad de la plataforma, al tiempo que permitiría funcionalidades más amplias.

### 3.2 TDEX para creadores de mercado

En la red TDEX, los *creadores de mercado* son entidades que proporcionan liquidez a los pares de activos que se negociarán en la plataforma de cambio y, por lo tanto, también pueden denominarse *proveedores de liquidez* (**Proveedor**). La función principal del Proveedor es mantener un par vinculado mutuamente de un activo cotizado (quote_asset) y un activo base (base_asset). Sin embargo, debe advertirse que esto se aplica a cualquier par de activos y no necesariamente a los vinculados al Bitcoin.

Como solución para el problema clásico de la [*doble coincidencia de deseos*](https://www.oxfordreference.com/view/10.1093/oi/authority.20110803095622703), TDEX permite que los creadores de mercado ejecuten endpoints *siempre activos*, al tiempo que revelan su dirección accesible públicamente utilizando cualquiera de los canales definidos en BOTD #2. Esto asegura mercados fácilmente disponibles para los traders, lo que aborda uno de los principales puntos débiles de las plataformas descentralizadas.

#### 3.2.1 Implementación de daemons

Para participar como proveedor, es preciso implementar un Daemon en la red, ya sea ejecutándolo a través de Docker o como entidad independiente (Más información en: [Procedimiento de implementación de daemons](https://docs.tdex.network/tdex-daemon.html)). Un daemon estándar en TDEX expone dos endpoints HTTP/2 gRPC, la **Interfaz del trader** (pública) y la **Interfaz del operador** (privada). Aunque la interfaz pública representa el puerto para los traders (por defecto: 9945), la interfaz privada (por defecto: 9000) se utiliza en las transacciones internas del creador de mercado. Además, para tener una seguridad óptima, [Blockstream Green](https://help.blockstream.com/hc/en-us/categories/900000056183-Blockstream-Green) o Liquid Wallet se incrusta previamente en cada daemon.

#### 3.2.2 Estrategias de creación de mercados

Uno de los elementos diferenciadores de TDEX es que proporciona múltiples opciones de creación de mercado para los proveedores, lo que amplía significativamente su alcance. En otras palabras, TDEX permite que los creadores de mercado elijan o creen sus estrategias, en lugar de imponer una u otra.

De forma predeterminada, el protocolo adopta una estrategia de *creación de mercado de función constante* (CFMM, por sus siglas en inglés) para determinar los precios de los activos. No obstante, los creadores de mercado también tienen la opción de implementar fuentes de precios *conectables* (externas) mediante una API personalizada. Teniendo en cuenta que la participación empresarial sería fundamental para el éxito de TDEX, las estrategias de creación de mercado personalizadas se encuentran entre las funcionalidades más cruciales de la plataforma, sobre todo porque mantiene simultáneamente la lógica de la elección de los usuarios. En otras palabras, mientras que los proveedores tienen la opción de seleccionar su estrategia de precios, los traders soberanos de la plataforma tienen la capacidad de elegir o rechazar estas estrategias.

#### 3.2.3 Tarifa de intercambio

Aunque el ratio de reserva *base_asset-quote_asset* cambia con cada operación, TDEX garantiza la coherencia del tamaño del mercado general cobrando una tarifa de intercambio mínima por cada operación y añadiéndola a las reservas. Teniendo en cuenta que el arbitraje provocará un flujo de transacciones uniforme, en aquellos casos en que el creador de mercado implemente una estrategia basada en AMM, los ingresos generados con esta tarifa deberían crecer con el tiempo.

Paralelamente, sin embargo, TDEX adopta el [mecanismo](https://en.bitcoin.it/wiki/PayJoin) [P2EP](https://en.bitcoin.it/wiki/PayJoin), por lo que minimiza el espacio de la cadena de bloques requerido por las transacciones, lo cual optimiza efectivamente la tarifa involucrada. Esto se hace para garantizar unas condiciones justas y equilibradas en el protocolo tanto para traders como para proveedores.

#### 3.2.4 Fondos de liquidez (implementación futura)

Más adelante, en su hoja de ruta prevista, TDEX implementaría una funcionalidad *sin custodia* que puede actuar como el sistema para que los daemons se conecten y agrupen sus activos. Una vez logrado, esto garantizaría una liquidez mayor y más uniforme en el protocolo, además de exponer un único endpoint para mayor comodidad de los usuarios. A su vez, TDEX podría adaptarse a demandas financieras que requieran una gran escala.

Así, el proveedor que cree un fondo será el *Pool Master* y otros proveedores podrán unirse a la *red de servicios distribuidos* para agregar liquidez. Como incentivo, el «pool master» tendrá la capacidad de determinar el precio base de los activos del fondo y los traders tendrán que buscar los precios al contado agregados del proveedor. Para cualquier activo dado, un proveedor podrá actuar por su cuenta o unirse a un fondo, pero no asumir ambas posiciones simultáneamente.

### 3.3 TDEX para traders

En el contexto de TDEX, el *mercado* es cualquier par de activos base y cotizado que se pueden intercambiar atómicamente. Como se menciona en BOTD #3, un **Proponente** tiene que iniciar intercambios en TDEX y, alternativamente, representa a un trader en la red. En otras palabras, un trader en TDEX es cualquier usuario que implementa completamente el Protocolo comercial (BOTD #4). Al hacerlo, se conecta con la interfaz del trader antes mencionada (el puerto público del daemon del proveedor) y acepta operar al precio de mercado estipulado.

En general, operar en TDEX es similar a hacerlo en cualquier otra plataforma basada en intercambios atómicos, lo que significa que el trader puede intercambiar proporciones iguales (por valor de mercado) de ambos activos en el par. Sin embargo, a diferencia de la mayoría de sus colegas en otras redes, el sistema de TDEX garantiza confidencialidad, liquidaciones más rápidas y retrasos mínimos o nulos. Además, al no tener custodia, TDEX alivia al usuario de las preocupaciones relativas a la pérdida de fondos por ataques e infracciones.

#### 3.3.1 Kits de desarrollo de software: Contribución de TDEX al código abierto para LiFi

Además de la interfaz de usuario predeterminada, el protocolo también permite a los usuarios implementar su cliente personalizado utilizando los kits de desarrollo de software (SDK, por sus siglas en inglés) de TDEX. En la fase inicial, esto se puede hacer usando [JavaScript](https://docs.tdex.network/tdex-sdk.html), pero en el futuro, TDEX tendrá SDK para Python, Go y Rust. Por otro lado, en la fase inicial, los traders interactúan con los proveedores utilizando la [interfaz de línea de comandos](https://docs.tdex.network/tdex-cli.html#install) (CLI, por sus siglas en inglés), hasta que se haga realidad el plan futuro para tener una aplicación móvil descentralizada.

Básicamente, estos SDK representan las contribuciones de TDEX a las capacidades de código abierto de la red, principalmente al capacitar a los desarrolladores versados en la implementación de API de Bitcoin y otras funcionalidades similares. En este sentido, la visión más amplia es impulsar las innovaciones dentro del ecosistema Liquid, sobre todo con el objetivo de fortalecer la generación de liquidez en la red.

### 3.4 Casos de uso

Una vez comentados los diversos elementos del ecosistema TDEX, veamos ahora algunos destacados y posibles casos de uso.

#### 3.4.1 Mercado secundario de Liquid Assets

En general, hay que tener en cuenta que los activos intercambiados en la red TDEX son esencialmente Liquid Assets. Por lo tanto, ser un mercado secundario de Liquid Assets se encuentra entre los principales casos de uso de la plataforma TDEX, al menos en las etapas iniciales.

En resumen, Liquid permite a sus usuarios «emitir» activos transferibles, que abarcan diferentes clases de activos: monedas fiduciarias tokenizadas y otras criptomonedas que no son BTC, tokens no fungibles (coleccionables), tokens de incentivo (recompensas), materias primas tokenizadas (por ejemplo, monedas de oro), etc. Cada Liquid Asset tiene un identificador de 64 caracteres, que se puede adjuntar con dominios legibles por humanos en la cadena de bloques publicando sus metadatos en el «Registro de activos» en Blockstream.info, es decir, en la versión de Liquid de un Explorador de bloques. El protocolo también permite la reemisión de tokens y la quema de tokens. En el contexto de TDEX, esto significa que los proveedores pueden crear mercados para cualquier par de L-Assets, lo que facilita las operaciones con estos activos. Del mismo modo, podría aprovecharse en transacciones y ventas con tokens no fungibles (NFT, por sus siglas en inglés).

En este punto, sin embargo, es imperativo tener en cuenta un aspecto crucial de la visión de TDEX, y es que TDEX no tendrá un token nativo, principalmente porque el proyecto está orientado a la comunidad y no prioriza ningún ánimo de lucro.

#### 3.4.2 Trading institucional y transferencia de fondos

Los usuarios y creadores de mercado de la red TDEX no tienen por qué ser necesariamente personas, sino que también pueden ser instituciones y empresas. Por lo tanto, la plataforma proporciona un canal seguro para que dicha organización opere con activos líquidos, que a su vez, deberían desempeñar un papel determinante en la mejora de las adopciones a largo plazo y en la ampliación de la comunidad.

Junto a esto, el conjunto de herramientas de código abierto de TDEX amplía aún más el alcance al establecer la posibilidad de que las empresas (pequeñas, medianas y grandes) implementen soluciones personalizadas para satisfacer sus necesidades financieras de manera descentralizada. De hecho, es en este sentido que el objetivo de TDEX de convertirse en una «red troncal» para Trustless Finance puede hacerse realidad.

## 4. Conclusión

Las preocupaciones por la privacidad y la seguridad se multiplican. Las obligaciones de cumplimiento están paralizando las plataformas de cambio centralizadas de varias maneras, mientras que las descentralizadas comprometen la seguridad y son presa de ataques informáticos, estafas e infracciones de varios tipos. En última instancia, como efecto combinado de estos factores, los usuarios están perdiendo su dinero o sus datos y, lo que es más importante, se ven privados de sus derechos básicos a la privacidad y la autonomía.

Desarrollada en este contexto, TDEX es un protocolo descentralizado que prioriza la privacidad y se implementa en Liquid Network. Principalmente un protocolo de negociación basado en intercambio atómico, la plataforma también tiene un conjunto de herramientas de código abierto que los desarrolladores pueden usar para implementar API personalizadas y otras soluciones en la red. En su conjunto, TDEX prevé convertirse en un protocolo troncal que facilite soluciones descentralizadas en Liquid Network y, a su vez, fortalezca la base de Trustless Finance como un espacio seguro, protegido y meritocrático para una comunidad global de usuarios y entusiastas del Bitcoin.

## Reconocimientos

Al embarcarse en un viaje hacia la construcción del futuro, varias personas y empresas han inspirado, asesorado y ayudado a TDEX. Al darnos cuenta de que el proyecto nunca sería posible sin ellas, queremos agradecer algunas de sus muchas contribuciones.

[Blockstream](https://blockstream.com/)

[Vulpem Ventures](https://vulpem.com/)

[Mohammad Musharraf](http://mohammadmusharraf.com/)

[Shiladitya Sinha](https://www.linkedin.com/in/shiladityasinhaofficial/)

Sobre todo, gracias a Satoshi Nakamoto
