
**Data:** 2024-10-14
**keyboards:** 
**links internos:** 
___

# Introdução

## História e evolução das linguagens de programação

A jornada das linguagens de programação, da linguagem de máquina até a programação orientada a objetos.

### 1. Primeira geração: Linguagem de máquina (1940s)

No inicio da era da computação, os programadores precisavam se comunicar com as máquinas usando a **Linguagem de máquina**, composta por sequências de 0s e 1s que representavam instruções diretamente executáveis pelo hardware. Era um processo extremamente trabalhoso, propenso a erros e específico para cada tipo de máquina. Imagine ter que decorar códigos binários para cada operação que você quisesse que o computador realizasse?!


### 2. Segunda geração: Linguagens Assembly (1950s)

A necessidade de tornar a programação mais humana levou ao surgimento das ***linguagens Assembly***. Elas usavam mnemônicos (abreviações) para representar as instruções de máquina, como "ADD" para adição e "MOV" para mover dados. Um programa chamado **assembler** traduzia essas instruções em código de máquina. Apesar de ser um passo à frente, ainda era uma linguagem de baixo nível, complexa e dependente da arquitetura da máquina.


### 3. Terceira geração: Linguagens de alto nível (1960s-1970s)

As **linguagens de alto nível** surgiram para tornar a programação mais próxima da linguagem humana e independente da máquina. Linguagens como **FORTRAN** (para cálculos científicos), **COBOL** (para aplicações comerciais) e **C** (para programação de sistemas) permitiam aos programadores escrever código de forma mais intuitiva e expressiva. Essas linguagens introduziram conceitos como **variáveis**, estruturas de controles (**if-else, loops**) e **funções**, aumentando a produtividade e a portabilidade do código.


### 4. Paradigmas de programação (1970s - presente)

Com o amadurecimento das linguagens de alto nível, surgiram diferentes **paradigmas de programação**, que são abordagens para organizar e estruturar o código. Alguns dos principais paradigmas são:

#### Programação imperativa:
Foca em descrever _como_ o programa deve realizar uma tarefa, especificando cada passo.
exemplos: **C**, **Pascal**.

#### Programação declarativa:
Foca em descrever o que o programa deve fazer, sem especificar os passos. 
Exemplos: **SQL**, **Prolog**.

#### Programação funcional:
Trata a computação como uma avaliação de funções matemáticas, evitando efeitos colaterais
Exemplos: **Lisp**, **Haskell**.

#### Programação Lógica:
Baseada em lógica formal e inferência, usada para resolver problemas através de regras e fatos.
Exemplo: **Prolog**.

### 5. A ascensão da Programação Orientada a Objetos (1980s - presente)

A **Programação orientada a objetos (POO)** revolucionou a forma como os programas são construídos. Ela introduziu conceitos como **classes**, **objetos**, **encapsulamento**, **herança** e **polimorfismo**, que permitem modelar o mundo real de forma mais natural e modular. Linguagens como **Smalltalk, C++, Java e Python** popularizaram a POO, oferecendo maior reusabilidade, manutenabilidade e escalabilidade de código.


A POO teve um impacto profundo no desenvolvimento de software, influenciando áreas como:

#### Interfaces gráficas:
Facilitando a criação de interfaces visuais mais complexas.

#### Desenvolvimento web:
Com frameworks como Java Spring e Ruby on Rails

#### Jogos:
Permitindo a criação de personagens e objetos interativos.

#### Banco de dados:
Com o surgimento de banco de dados orientados a objetos.


## O que é Programação Orientada a Objetos?

A programação orientada a objetos (POO) é um paradigma de programação que organiza o código em unidades chamada "**Objetos**". 
Imagine que cada objeto é como uma caixa que contém dados (**variáveis**) e ações (**funções**, que em POO chamamos de **métodos**) que operam sobre esses dados. Essa forma de organizar o código é muito poderosa e se assemelha à maneira como pensamos sobre o mundo real, tornando os programas mais fáceis de entender, manter e reutilizar.


### Conceitos fundamentais:

#### classes:
pense em uma classe como um molde ou um projeto para criar objetos. Ela define características (**atributos**) e comportamentos (**métodos**) que os objetos dessa classe terão.
Por exemplo, a classe "cachorro" pode ter atributos como "nome", "raça" e "idade", e métodos como "latir" e "correr".

#### objetos: 
São instâncias de uma classe. Usando o exemplo anterior, "Rex"  seria um objeto da classe "cachorro", com seus próprios valores para nome, raça e idade.

#### atributos:
São as características de um objeto, como a cor dos olhos de uma pessoa ou a marca de uma carro.

#### métodos:
São as ações que um objeto pode realizar, como um pássaro voando ou um carro acelerando.


### Pilares de POO:

#### Abstração:
É a capacidade de representar as características essenciais de um objeto, sem se preocupar com os detalhes internos. Pense no volante de um carro: você o utiliza para dirigir sem precisar saber como o mecanismo de direção funciona por baixo do capô.

#### Encapsulamento
Esconde os detalhes internos de um objeto e controla o acesso aos seus dados. isso portege os dados e simplifica a interação com o objeto. 
Imagine uma TV: você interage com ela usando um controle remoto, sem precisar acessar os circuitos internos.

#### Herança:
Permite criar novas classes a partir de classes existentes, herdando seus atributos e métodos. Isso promove a reutilização de código e facilita a criação de hierarquias de classes. 
Por exemplo, a classe "cachorro" pode herdar a classe "animal", herdando atributos como "peso" e "altura".

#### Polimorfismo:
Permite que objetos de classes diferentes respondam à mesma mensagem de maneiras diferentes.
Imagine o método "emitir som": um cachorro late, um gato mia e um pássaro canta, mesmo que todos respondam ao mesmo método.



### Vantagens da POO:

#### Modularidade:
Divide o programa em partes menores e mais gerenciáveis.

#### Reusabilidade:
Permite reutilizar código em diferentes partes do programa ou em outros projetos.

#### Manutenibilidade:
Facilita a manutenção e atualização do código.

#### Escalabilidade:
Permite que o programa cresça e evolua com mais facilidade. 




