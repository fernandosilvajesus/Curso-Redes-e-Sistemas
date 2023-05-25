# Redes e Sistemas

## O que são redes?

Redes são um conjunto de dois ou mais dispositivos eletrônicos conectados entre si, que trocam informações por meio de uma linguagem pré-estabelecida chamada protocolo.

Essa conexão pode ocorrer de duas formas:
- Conexão física via cabos de par trançados, Coaxial ou fibra óptica.
- Via wireless através de rádio frequência, Bluetooth ou infravermelho.

## Origem das redes

As redes de computadores tiveram sua origem durante a Guerra Fria, mais especificamente na década de 1960, em um contexto de rivalidade entre os Estados Unidos e a União Soviética. O DARPA (Defense Advanced Research Projects Agency), que é o Departamento de Defesa dos Estados Unidos, desempenhou um papel fundamental no desenvolvimento das redes nesse período.

O projeto mais notável desenvolvido pelo DARPA foi o ARPANET (Advanced Research Projects Agency Network), criado em 1969. O ARPANET foi a primeira rede de computadores a utilizar comutação de pacotes e protocolos de comunicação para interligar computadores em diferentes locais. Essa iniciativa foi essencial para o surgimento da Internet como a conhecemos hoje.

As redes de computadores se comunicam entre si por meio de protocolos, que são conjuntos de regras e padrões que definem como os dados devem ser transmitidos, recebidos e interpretados. Alguns órgãos reguladores desempenham um papel importante na padronização e na regulamentação das comunicações entre as redes.

A IANA (Internet Assigned Numbers Authority) é responsável por coordenar a atribuição global de endereços IP e números de protocolo, além de supervisionar o sistema de nomes de domínio (DNS). Ela também trabalha em conjunto com as RIRs (Regional Internet Registries) para a alocação e distribuição de blocos de endereços IP.

A ISO (International Organization for Standardization) é uma organização internacional que estabelece normas em diversas áreas, incluindo as redes de computadores. A ISO define padrões e recomendações para a comunicação entre redes, protocolos de rede, arquiteturas de rede e muito mais.

## Infraestrutura de redes e os principais equipamentos

- NIC (Network Interface Card): Placa de rede responsável pela conexão do computador com o cabo de rede Ethernet ou por receber as conexões wireless.

- Hub: Dispositivo que permite a conexão entre dispositivos por meio de cabos de par trançados RJ45.

- Switch: Responsável pela comutação dos quadros entre os dispositivos, permitindo uma conexão de ponta a ponta.

- Roteador: Tem a responsabilidade de procurar as melhores rotas na internet para entregar os pacotes do remetente ao destinatário ao menor tempo possível.

- Modem: Equipamento responsável pela modulação e demodulação de internet, podendo desempenhar também o papel de roteador em residências.

## Cabeamento Estruturado

O cabeamento estruturado é a organização padronizada dos cabos e periféricos em uma rede, proporcionando melhor desempenho e organização.

Normas que determinam como o cabeamento deve ser feito:
- NBR 14.565 (norma brasileira)
- ANSI/TIA 568 (norma internacional)
- ANSI/TIA 569 (norma internacional)

### Cabos

- Cabo de par trançado: Dividido em categorias que determinam a velocidade de transmissão e o alcance em metros. Existem dois tipos: UTP (não possui isolamento) e STP (possui isolamento).

- Cabo coaxial: Composto por fios de cobre, sendo utilizado em conexões de modems, telefones e TVs a cabo.

- Cabo de fibra óptica: Oferece alta velocidade de transmissão de dados e é composto por pedaços de vidro que permitem a propagação de raios de luz.

### Rack e sua importância

O rack é um armário utilizado para hospedar os equipamentos de hardware, como switches, roteadores e fibras ópticas, e para organizar os cabos em patch panels. Ele desempenha um papel essencial em data centers e infraestruturas de redes.


## Modelo OSI

<p>
O modelo OSI (Open Systems Interconnection) é um modelo de referência que descreve como os sistemas de rede se comunicam entre si. Ele é dividido em sete camadas, cada uma com funções específicas. A comunicação no modelo OSI ocorre da seguinte forma:
</p>

1. **Camada Física:** Lida com a transmissão física dos dados, convertendo-os em sinais elétricos, de luz ou de rádio.

2. **Camada de Enlace:** Responsável pela transferência confiável de dados entre nós adjacentes na rede. Detecta e corrige erros que podem ocorrer na camada física.

3. **Camada de Rede:** Lida com o roteamento dos pacotes de dados pela rede, determinando o melhor caminho para a entrega correta dos dados.

4. **Camada de Transporte:** Fornecer serviços de comunicação fim a fim, garantindo a entrega correta e ordenada dos dados.

5. **Camada de Sessão:** Estabelece, gerencia e encerra as sessões de comunicação entre aplicativos em diferentes dispositivos.

6. **Camada de Apresentação:** Lida com a representação dos dados, garantindo que sejam compreensíveis pelo destinatário.

7. **Camada de Aplicação:** Fornece interfaces para que os aplicativos acessem a rede e interajam com os usuários.

No modelo OSI, a conexão pode ser estabelecida tanto de baixo para cima (da camada física à camada de aplicação) quanto de cima para baixo (da camada de aplicação à camada física). Isso ocorre por meio do encapsulamento dos dados em cada camada conforme eles são transmitidos pela rede.


# TCP/IP

O TCP/IP (Transmission Control Protocol/Internet Protocol) é um conjunto de protocolos que define a forma como a comunicação ocorre na Internet. Ele é baseado em quatro camadas principais:

- **Camada de Interface de Rede**: Lida com a transmissão física dos dados, semelhante à camada física no modelo OSI.
- **Camada de Internet**: Equivalente à camada de rede no modelo OSI. Realiza o roteamento dos pacotes na rede.
- **Camada de Transporte**: Corresponde à camada de transporte no modelo OSI. Fornece serviços de comunicação fim a fim, garantindo a entrega correta dos dados.
- **Camada de Aplicação**: Combina as camadas de sessão, apresentação e aplicação do modelo OSI. Fornece serviços de comunicação de alto nível para os aplicativos na rede.

O TCP/IP é amplamente utilizado na comunicação em redes de computadores, especialmente na Internet. Ele fornece um conjunto de protocolos robustos e escaláveis para transmitir dados de forma confiável e eficiente.

Em comparação com o modelo OSI, o TCP/IP tem uma abordagem mais simplificada, mas ainda oferece funcionalidades essenciais para a comunicação em rede.


## IPv4 e IPv6

O IP (Internet Protocol) é o protocolo responsável pelo endereçamento dos pacotes de rede na camada 3 do modelo OSI. Ele gera um endereço para o seu computador ou servidor quando está conectado à Internet. Existem atualmente dois formatos principais:

### IPv4

O IPv4 é o formato mais comum de endereço IP. É representado por quatro conjuntos de números separados por pontos, como por exemplo: 192.168.0.1. Cada conjunto de números, também chamado de octeto, pode variar de 0 a 255. O IPv4 possui um espaço de endereçamento de 32 bits, o que permite aproximadamente 4 bilhões (ou 4 milhões de conexões) de endereços únicos.

### IPv6

O IPv6 é um formato de endereço IP mais recente e foi desenvolvido para superar a limitação de endereços do IPv4. Ele é representado por oito conjuntos de quatro dígitos hexadecimais, separados por dois pontos, como por exemplo: 2001:db8:3333:4444:5555:6666:7777:8888. Cada conjunto de quatro dígitos hexadecimais corresponde a 16 bits, totalizando 128 bits de espaço de endereçamento. Isso permite um número extremamente grande de endereços, aproximadamente 1 decilhão (ou 1 trilhão de bilhões) de conexões únicas.

## NAT (Network Address Translation)

O NAT é uma função utilizada em roteadores que permite a tradução de endereços IP entre uma rede local (privada) e a Internet. Ele funciona permitindo que conexões sejam feitas da rede privada para recursos na Internet. Por exemplo, um cliente da rede local acessando um servidor de FTP na Internet. Nesse caso, o cliente estabelece uma conexão com o servidor FTP usando um programa cliente, e o roteador realiza a tradução de endereços IP para permitir a comunicação.


