
**Data:** 2024-09-30
**keyboards:** 
**links internos:** 
___

# O que é a Linguagem Python? 

Python é uma linguagem de alto nível, interpretada, de tipagem dinâmica e multiparadigma.
Criada por Guido van rossum e lançada pela primeira vez em 1991, Python é projetada para ser simples e legível.

As instruções das linguagens de alto nível são bastante abstratas e não estão relacionadas à arquitetura do computador diretamente.


## ***[[Interpretada]]***

 Python é uma linguagem interpretada, o que significa que o código é executado linha por linha. Isso permite uma rápida [[prototipagem]] e facilita o processo de **[[Debugging]]**.



## ***[[Tipagem dinâmica]]***:
   
   Não é necessário declarar o tipo de uma variável. O tipo é determinando em tempo de execução, o que permite maior flexibilidade.


## ***[[Multi-paradigma]]***: 
 
 Suporta programação orientada a objetos, funcional e imperativa, permitindo aos desenvolvedores escolherem o estilo que melhor se adapta ao problema.


___

# [[Variáveis em python]]

Variáveis em Python são como recipientes que armazenam dados, como números, textos ou listas. Elas permitem que você nomeie e acesse esses dados facilmente no seu código, tornando-o mais organizado e flexível. Pense nelas como etiquetas que você coloca em diferentes tipos de informação para encontrá-las depois.



## [[Conceito de amarração (binding)]]

Amarração em Python é basicamente como dar um nome a um objeto na memória do computador. Imagine que você guarda um objeto numa caixa e coloque uma etiqueta nela. A etiqueta é o nome (variável) e a caixa com o objeto é o espaço na memória. Essa etiqueta te permite acessar e usar o objeto no seu código.

___

# Condicionais em python

Em Python, uma condicional é como uma pergunta que você faz ao programa.
Se a resposta for "sim" (verdadeira), o programa faz uma coisa. Se a resposta for não (falsa), ele pode fazer outra coisa ou simplesmente seguir em frente.


## Condição simples e composta

Em python, as condições são usadas para controlar o fluxo do seu programa, permitindo que ele tome decisões. Elas podem ser simples ou compostas:

### Condição Simples

- Usa apenas a palavra-chave ==if==.
- Executa um bloco de código **Se** a condição for verdadeira. se for falsa, pula o bloco.
- é como uma porta que só abre se você tiver a chave certa.

```
idade = 20
if idade >= 18:
  print("Você pode dirigir!")
```

### Condição composta

- Usa ==if== e ==else==.
- Executa um bloco de código **se** for verdadeira e **outro** bloco for falsa.
- É como um caminho com uma bifurcação: pode pode pegar um caminho se a condição for verdadeira e outra se for falsa.

```
idade = 15
if idade >= 18:
  print("Você pode dirigir!")
else:
  print("Você ainda não pode dirigir.")
```

Em resumo, a diferença principal é que a condição ***composta*** sempre executa um dos blocos de código, enquanto a ***simples*** pode não executar nenhum.




