
**Data:** 2025-02-27
**keyboards:** 
**links internos:** 
___

# 1. O que é Cloud Computing?

Cloud Computing é um paradigma que permite acessar e gerenciar recursos computacionais remotamente, sem a necessidade de manter infraestrutura física própria. Isso é possivel por meio de [[Data Centers]] distribuídos globalmente, que oferecem capacidade computacional sob demanda.

![[Pasted image 20250227133544.png]]



# 2 Conceitos Fundamentais de Cloud Computing

Os conceito se baseia em três pilares principais:

## Virtualização

A virtualização permite criar versões virtuais de servidores, redes e armazenamento, otimizando o uso de hardware físico.

Principais Tecnologias:

- **Hypervisors**: Software que gerencia máquinas virtuais (VMware ESXI, Hyper-V, KVM).

- **Conteiners:** tecnologia mais leves que VMs (Virtual machines), utilizando o mesmo kernel do sistema operacional (Docker, Kubernetes).



## Escalabilidade e Elasticidade 

- **Escalabilidade:** Capacidade de aumentar recursos conforme a demanda. pode ser *Vertical* (mais CPU/RAM em um servidor) ou *Horizontal* (adicionar mais servidores).

- **Elasticidade:** ajuste dinâmico da infraestrutura para atender flutuações  na carga de trabalho.


## Segurança na nuvem

- **Controle de acesso**: IAM (Identity and Acess Magenement) para definir permissões.

- **Criptografia:** proteção de dados em trânsito e em repouso.

- **Firewalls e WAF**: Barreiras de proteção contra ataques externos.


## Armazenamento na Nuvem 

- **Bloco:** semelhante a um HD virtual ( ex: Amazon EBS, Azure Disk Storage).

- **Objeto:** para armazenar grandes volumes de dados não estruturados (ex: Amazon S3, Google Cloud Storage).

- **Arquivo**: sistemas de arquivos compartilhados (ex: Amazon EFS, Azure Files).


## Rede e conectividade 

- **VPC (Virtual Private Cloud):** Redes isoladas dentro da nuvem pública.

- **Load Balancer**: distribui tráfego entre servidores para evitar sobrecarga.

- **CDN (Content Delivery Network)**: acelera a entrega de conteúdo globalmente.



# 3. Modelos de Implantação da Nuvem

Existem diferentes modelos de implantação de nuvem, dependendo do nível de controle, segurança e disponibilidade necessários:


## Nuvem Pública

As nuvens públicas são aquelas nas quais os provedores de serviços disponibilizam todos os recursos, como computação, armazenamento e aplicativos para o público em geral pela internet. Qualquer usuário pode efetuar login e usar esses serviços. Você paga pelo número de recursos que usa. Nesse modelo, os Usuários possuem menos controle sobre seus dados. 

**Como funciona**:
- Um provedor de serviços de nuvem terceirizado é responsável por fornecer, operar e gerenciar os recursos de nuvem

- Os recursos de nuvem são disponibilizados pela internet

- Os usuários podem acessar os serviços e gerenciar suas contas através de um navegador da web

- **Vantagens**: 
	- escalabilidade 
	- performance
	- custo reduzido 
	- manutenção gerenciada pelo provedor.

- **Desvantagens**: 
	- menor controle sobre segurança e configuração.


## Nuvem Privada

As nuvens privadas são ambientes de nuvem construídos exclusivamente para um único usuário, ou uma única empresa, normalmente localizados por trás do firewall do usuário. 

- Infraestrutura dedicada a uma única organização, podendo estar hospedada localmente ou em um data center terceirizado.

- Exemplo: VMware vsphere, openStack, soluções privadas de AWS e Azure.

- **Vantagens**: Maior controle e segurança, melhor personalização.

- **Desvantagens:** custo mais alto e necessidade de gerenciamento interno


## Nuvem Híbrida 

As nuvens híbridas são aquelas constituídas pelos serviços da nuvem pública e privada. Alguns serviços são hospedados na nuvem privada, enquanto outras na nuvem pública. Assim, a empresa pode manter dados cruciais na nuvem privada e outros dados na nuvem pública, aproveitando o melhor dos dois mundos.

- Combina nuvem Pública e privada, permitindo que dados e aplicativos sejam compartilhados entre ambas.

- Exemplo: Uma empresa pode rodar workloads sensíveis em nuvem privada e usar a nuvem pública para escalabilidade.

- **Vantagens:** flexibilidade, segurança aprimorada, otimização de custos

- **Desvantagens**: maior complexidade na configuração e gestão.


## Multicloud

- Uso de múltiplas nuvens públicas de diferentes fornecedores para evitar dependência de um único provedor

- *Exemplo:* Usar a AWS para hospedagem de aplicativos e Google cloud para machine learning

- **Vantagens**: redundância, otimização de custos, maior confiabilidade.

- **Desvantagens**: complexidade no gerenciamento, desafios na integração.



# 4. Modelos de serviço em cloud 

Os serviços em nuvem são classificados em três modelos principais:


## **IaaS** (infraestrutura como serviço)

- Fornece infraestrutura de TI como servidores, redes, armazenamento e sistemas operacionais sob demanda.

- *Exemplo:* Amazon EC2, Google Computer Engine, Azure Virtual Machines.

- **Vantagens**: controle sobre a infraestrutura, flexibilidade na configuração.

- **Desvantagens**: exige conhecimento técnico para gerenciamento.


## **PaaS** (plataforma como serviço)

- Oferece um ambiente de desenvolvimento pronto, incluindo sistemas operacionais, bancos de dados e ferramentas de desenvolvimento.

- *Exemplo*: Google App Engine, AWS Elastic Beanstalk, Azure App services.

- **Vantagens**: Acelera o desenvolvimento de aplicativos, reduz a complexidade operacional.

- **Desvantagens**: menor controle sobre infraestrutura subjacente.


## **SaaS** ( Software como serviço)

- Aplicações prontas para uso acessadas pela internet sem necessidade de instalação ou manutenção

- *Exemplo:* Google drive, Dropbox, office 365, Salesforce.

- **Vantagens**: Fácil acesso e uso, sem necessidade de manutenção.

- **Desvantagens**: dependência do provedor para atualizações e disponibilidade. 




![[Pasted image 20250227134434.png]]

## Reponsabilidades para cada categoria de Serviço

![[Pasted image 20250312170245.png]]


# 7. Tecnologias e Ferramentas Populares

- **AWS (Amazon Web Services)**: Líder do mercado com vasta gama de serviços.

- **Microsoft Azure**: Forte presença no setor corporativo. 

- **Google Cloud Platform (GCP)**: destaque em machine learning e big data.

- **Kubernetes**: orquestração de containers para aplicações escaláveis. 

- **Terraform**: gerenciamento de infraestrutura como código.
