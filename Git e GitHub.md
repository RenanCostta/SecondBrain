
**Data:** 2024-09-27
**keyboards:** 
**links internos:** 
___

# GIT

## O que é:

Git é um software de versionamento para rastrear alterações em qualquer conjunto de arquivos, geralmente usado para coordenar o trabalho entre programadores que desenvolvem o código-fonte de forma colaborativa durante o desenvolvimento de Software. Seus objetivos incluem velocidade, integridade de dados e suporte para fluxos de trabalho Não lineares distribuídos.

## Por que preciso usar GIT:

1. Salvar múltiplas revisões do mesmo projeto em um único diretório. Chega de v1, v2, v2_final.
2. Trocar de versões em um simples comando.
3. Trabalhar simultaneamente em 2 ou mais "features" diferentes sem bagunçar o código original do projeto.
4. colaborar com outros programadores no mesmo time.

## Repositório GIT

Essencialmente Git repositório é um diretório chamado .Git dentro do seu projeto.

Este repositório rastreia todas as mudanças feitas nos arquivos do seu projeto, construindo um histórico ao longo do tempo.

## Commit

No Git, um commit é um comando que captura um instantâneo das alterações feitas em um projeto, registrando no repositório local.

Importante usar o commit apenas para os marcos importantes no seu projeto, evite commitar coisas banais.

Para você realizar o commit, o arquivo primeiro precisa passar por 3 estágios. são eles:

## Logs

Em Git, logs referem-se ao histórico de commits de um repositório. Os comandos principais para visualizar esse logs são:

- git log
- git log --oneline | logs de forma resumida , uma linha por commit
- git log -n2 | visualizar as duas ultimas mudanças
- git log -n2 --oneline
- git log --oneline --graph --all | para visualizar branches
- git log --exemple.txt | exibir logs de um arquivo específico
- git log -p | ver as mudanças feitas em cada commit
- git revert HEAD | desfazer o ultimo commit

O `git log` é útil para rastrear alterações, entender o histórico do projeto e até mesmo desfazer mudanças caso necessário.

### 3 Estágios do Commit

#### MODIFIED

Arquivos alterados

#### STAGING

Arquivos prontos para serem enviados.

Mas por que passar por esse processo? por que não ir direto proo commited?  
bom, é simples...  
Isso é por segurança. por exemplo:  
você alterou 10 arquivos no seu projeto, mas se não estiver seguro das alterações de todos eles, mas de apenas um arquivo em especial, você pode commitar apenas ele. coloca ele no STAGING e "Commita".

#### COMMITED

Arquivos enviados "Commited"

## Branch 

Um branch no Git é uma ramificação do código principal que permite aos desenvolvedores trabalhar em áreas isoladas para desenvolver recursos, corrigir erros ou experimentar novas ideias


# Git bash comands

## Conventional commits

![[Pasted image 20250227153129.png]]





# GitHub 
## O que é GitHub

GitHub, Inc. é um provedor de hospedagem na internet para desenvolvimento de software e controle de versão usando o GIT. Ele oferece o controle de versão distribuída e a funcionalidade de gerenciamento de código-fonte do Git, além de seus próprios recursos. Mas hoje em dia funciona muito mais que isso. quase que como uma Rede social para desenvolvedores.


## o GitHub serve para

1. "Hostear" o seu código em um local seguro.
2. Compartilhar seu projeto facilmente com outros devs.
3. Outros devs podem colaborar com o seu projeto.
4. Entre outras funcionalidades...






