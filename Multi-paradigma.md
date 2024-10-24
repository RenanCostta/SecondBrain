
**Data:** 2024-09-30
**keyboards:** 
**links internos:** 
___

# O que é multi-paradigma?

A programação multi-paradigma em python refere-se à capacidade da linguagem de suportar vários paradigmas de programação diferentes, permitindo que os desenvolvedores escolham o estilo ou combinação de estilos de programação que melhor se adequam ao problema que estão resolvendo, Vamos aprofundar o conceito e explicar como o python implementa isso:

## Os principais paradigmas suportados por python

1. ***programação imperativa:*** 
   - **Descrição:** A programação imperativa é um paradigma onde o código é escrito como uma sequência de instruções ou comando que o computador executa na ordem especificada. O foco está em "como" o programa deve realizar suas tarefas.
   
   - **Características em python:** Python permite criar scripts passo a passo que modificam o estado do rpograma por meio de variáveis e loops.
   
   - **Exemplo:**

```
total = 0 
for i in range(1,6):
	total += i
print(total)
```

- **quando usar:** Ideal para tarefas sequenciais ou scripts que precisam de controle explicito do fluxo.


2. ***[[Programação funcional]]***
   - **Descrição:** Este paradigma trata a computação como a avaliação de funções matemáticas e evita mudanças de estados dados mutáveis. 
   - **Recursos em python:** Python oferece suporte a a programação funcional por meio de funções como ```map()```, ```filter()```. ```reduce()``` e construções como ```lambda``` para reuniões anônimas. Além disso, Python possui suporte para a imutabilidade, embora não seja tão rígido quanto outras linguagens funcionais (por exemplo, Haskell).
   - **quando usar?** bom, é útil em tarefas de processamento de dados, transformações ou quando a imutabilidade é aleatória para evitar efeitos colaterais.


3. ***[[Programação orientada a objetos(POO)]]*** 
   - **Descrição:** POO é um paradigma que organiza o código em torno de "objetos" que encapsulam dados (atributos) e comportamentos (métodos). A ideia é modelar conceitos do mundo real e suas interações dentro do código.
   - **Características em python:** Python permite a criação de classes e objetos, herança, polimorfismo, encapsulamento e outras características do POO. embora python não imponha o uso estrito de orientação a objetos, ele facilita a adoção do paradigma.
   - **Quando usar?** Ideal para modelar sistemas complexos com múltiplas entidade que interagem sobre si.