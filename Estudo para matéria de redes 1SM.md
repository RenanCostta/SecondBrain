
**Data:** 2024-10-02
**keyboards:** 
**links internos:** 
___

# o que são redes, internet, protocolos.

## Redes de computadores:

Imagine um conjunto de ilhas. Para que as pessoas nessas ilhas se comuniquem e troquem recursos, elas precisam de pontes, barcos ou outras formas de conexão. Uma rede de computadores funciona de maneira similar. Ela conecta dispositivos como computadores, servidores, impressoras, smartphones, etc., permitindo que eles "conversem" entre si.

**Mas como essa conversa acontece?**

Através da troca de dados. Esses dados podem ser qualquer tipo de informação: mensagens de texto, arquivos, fotos, vídeos, etc. Para que essa troca aconteça de forma organizada, as redes usam **meios de transmissão** (as "pontes" entre as ilhas) e **protocolos** (as "regras de navegação").

### Meios de transmissão:

- **Físicos**:
	- ***Cabos***: Os dados "viajam" através de fios, como cabos de rede(==ETHERNET==) ou fibra ótica (mais rápida e com maior capacidade)
	- ***Ondas de Rádio***: Usadas em redes Wi-fi e bluetooth, os dados são transmitidos sem fio.
- **lógicos**: 
	- ***Protocolos***: Como veremos a seguir, eles definem as regras da comunicação.

### Tipos de redes: 

As Redes podem ser classificadas de acordo com sua abrangência geográfica:

- **LAN (local Area network)**: 
	Redes locais, de curta distância, como em uma casa, escritório ou escola. Geralmente usam cabos ou Wi-fi.
- **MAN (Metropolitan Area Network)**
	Redes que abrangem uma cidade ou região metropolitana,
- **WAN (Wide Area Network)**: 
	Redes de longa distância, que podem se estender por países ou continentes. A internet é o maior exemplo de WAN.

### Componentes em uma Rede

- **Hardware**: 
	- ***placas de rede***: permitem que o dispositivo se conecte à rede)
	- ***Roteadores***: encaminham dados entre as redes.
	- ***Switches***: conectam dispositivos dentro de uma rede.
	- ***Hubs***: concentradores de conexões.
	- cabos
	- antenas
	- etc..
- **Software**:
	sistemas operacionais de rede (gerenciam a rede), protocolos de comunicação, aplicativos de rede, etc...

## Internet

A internet é como um arquipélago gigante, onde cada ilha é uma rede menor (LAN, MAN) Essas Ilhas se conectam através de backbones, que são links de alta velocidade. Assim, a internet forma uma rede mundial de computadores, permitindo a comunicação global. 

### Serviços de Internet

A internet oferece uma variedade de serviços, como:

- WWW (World Wide Web): 
	Sistema de documentos interligados (páginas web) que você acessa os navegadores 
- E-mail: 
	permite enviar e receber mensagens eletrônicas.
- FTP (File Transfer Protocol): 
	Usado para transferir arquivos entre computadores.
- Streaming: 
	Transmissão de áudio e vídeo em tempo real.
- VoIP (Voice over IP): 
	Permite fazer chamadas eletrônicas pela internet.

### endereçamento na internet

Cada dispositivo na internet possui um endereço IP (Internet Protocol) único, como um "número de telefone" que identifica na rede. Para facilitar a memorização, usamos nomes de domínios, que são traduzidos para endereço IP.

## Protocolos

Imagine que cada ilha  no nosso arquipélago tem suas próprias leis e costumes. Para que a comunicação entre as ilhas funcione, é preciso que todos concordem com um conjunto de regras comuns, Os protocolos são essas "Regras de comunicação" na internet.

Eles definem como os dados devem ser formatados, endereçados, transmitidos, recebidos e verificados. Existem diversos protocolos, cada um com uma função específica:

- **TCP (Transmission Control Protocol):** 
	Garante a entrega confiável dos dados, dividindo-os em pacotes e verificando se todos chegaram corretamente
- **IP (Internet Protocol):** 
	Responsável por endereçar os pacotes de dados e encaminhá-los pela rede.
- **HTTP (Hypertext Transfer Protocol)**: 
	Usado para a comunicação entre navegadores e servidores Web.
- **HTTPS**: 
	Versão segura do HTTP, que criptografada a comunicação para proteger os dados.
- **FTP (File Transfer Protocol):** 
	permite a transferência de arquivos entre computadores.
- **SMTP (Simple Mail Transfer Protocol)**:
	Usado para enviar e-mails.
- **POP3 (Post Office Protocol Version 3) e IMAP (Internet Message Access Protocol):** 
	Usados para receber E-mails.

## Resumo:


Redes, Internet e protocolos são conceitos interligados que formam a base da comunicação digital no mundo moderno. As redes conectam dispositivos, a internet conecta redes, e os protocolos garantem que a comunicação flua de forma organizada e eficiente.





# Modelo Osi e Arquitetura TCP/IP

Ambos são modelos de referência em redes de computadores, mas com algumas diferenças importantes.

## Modelo OSI (Open Systems Interconnection)

Imagine uma linha de produção de um a fábrica. Cada setor tem uma função específica para que o produto final seja criado. O modelo OSI funciona de forma similar, dividindo a comunicação em rede de **sete camadas**. cada uma com responsabilidades bem definidas. Essas divisão facilita a compreensão, o desenvolvimento e a resolução de problemas em redes.

### As setes camadas do Modelo OSI:

#### 1. Camada Física: 

- **Conceito:** A camada mais básica, responsável pela transmissão de bits brutos (0s e 1s) através do meio físico. Pense nela como a "encanadora" da rede, que cuida dos fios, cabos, conectores e sinais elétricos ou ópticos.
- **Detalhes:**
    - **Meios de Transmissão:** Cabos de cobre (par trançado, coaxial), fibra óptica, ondas de rádio (Wi-Fi, Bluetooth), etc.
    - **Codificação de Sinais:** Como os bits são representados fisicamente (níveis de voltagem, pulsos de luz, modulação de frequência).
	- **Sincronização:** 
		Como o emissor e o receptor sincronizam seus relógios para interpretar os sinais corretamente
	- **Topologia de rede:**
		Como os dispositivos estão fisicamente conectados (barramento, estrela, anel, etc..)
- **Funcionamento:**
	A camada física recebe os bits da camada de enlace de dados e os converte em sinais elétricos ou ópticos para a transmissão. No receptor, ela converte os sinais de volta em bits e os envia para a camada de enlace de dados.
	- **Exemplos**: 
		- **Especialidades do cabo**:
			Categoria do cabo Ethernet (==cat 5e==, ==cat 6==), tipo de fibra óptica (monomodo, multimodo)
		- **Padrões Wi-fi**: 802.11a/b/g/n/ac, que definem frequências, taxas de dados e modulação.
		- **Interfaces de rede:**
			Ethernet (RJ-45, USB, SERIAL, etc...)

#### 2. Camada de Enlance de dados:

- **Conceitos:** 
	Organiza os bits em quadros (frames) e controla o acesso ao meio físico. imagine que um carteiro que empacota as cartas (dados) e gerencia a fila de envio.
- **Detalhes:**
	- **Endereçamento fixo (MAC address):**
		Cada dispositivo na rede possui um endereço MAC único, que o identifica na camada de enlace de dados.
	- **Controle de acesso ao meio (MAC):**
		Protocolos que definem como os dispositivos compartilham o meio físico, evitando colisões (ex: CSMD/CD para ethernet)
	- **Detecção e correção de erros:**
		Mecanismo para detectar e corrigir erros na transmissão, como ==checksum== e ==CRC==.
	- **Segmento e Reassembly:**
		Divide os dados em quadros menores para facilitar a transmissão e os remonta no receptor
- **Funcionamento:**
	A camada de enlace de dados recebe os dados da camada de rede e os encapsula em quadros, adicionando o endereço MAC de origem e destino. No receptor, ela remove o cabeçalho do quadro e envia os dados para a camada de rede.
- **Exemplos:**
	- **Ethernet:** 
		Protocolo de rede local mais comum, que usa o método ==CSMA/CD== para controle de acesso ao meio.
	- **Wi-Fi:**
		Protocolo de rede sem fio que usa diferentes métodos de acesso ao moi, como ==CSMA/CA==. 
	- **PPP (Point-to-Point Protocol)**:
		Usado para conexões ponto-a-ponto, como ==dial-up==.


#### 3. Camada de rede

- **Conceito:**
	Responsável pelo roteamento dos pacotes de dados pela rede

# Resumo das 7 camadas OSI

O modelo OSI é um modelo conceitual que divide a comunicação em rede de sete camadas, cada uma com função especificas:

### 1. Física
Transmissão de bits brutos pelo meio físico (cabos, fibra óptica) define voltagem, conectores e taxa de transmissão

### 2. Enlace
Organiza Bits em quadros e gerencia o acesso ao meio físico. faz o controle de fluxo e detecção de erros. ex: ==Ethernet==, ==Wi-Fi==.

### 3. Rede
Roteamento dos pacotes de dados pela rede. Define endereços IP e escolhe o melhor caminho para o destino.

### 4. Transporte 
Garante a comunicação fim-a-fim entre as aplicações. Controla o fluxo de dados e garante a entrega confiável. ex: ==TCP==, ==UDP==.


### 5. Sessão
Estabelece, gerencia e encerra sessões de comunicação entre aplicações.


### 6. Apresentação
Formata os dados para a aplicação, incluindo criptografia, compressão e conversão de formatos.


### 7. Aplicação
Interface direta com o usuário. Fornece serviços de rede para as aplicações. Ex: navegadores, e-mail.