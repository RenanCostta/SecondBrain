
**Data:** 2025-03-15
**keyboards:** 
**links internos:** 
___

# Condição Simples

- Usa apenas a palavra-chave ==if==.
- Executa um bloco de código **Se** a condição for verdadeira. se for falsa, pula o bloco.
- é como uma porta que só abre se você tiver a chave certa.

```
idade = 20
if idade >= 18:
  print("Você pode dirigir!")
```

# Condição composta

- Usa ==if== e ==else==.
- Executa um bloco de código **se** for verdadeira e **outro** bloco for falsa.
- É como um caminho com uma bifurcação: pode pode pegar um caminho se a condição for verdadeira e outra se for falsa.

```
idade = 15
if idade >= 18:
  print("Você pode dirigir!")
else:
  print("Você ainda não pode dirigir.")
```

Em resumo, a diferença principal é que a condição **_composta_** sempre executa um dos blocos de código, enquanto a **_simples_** pode não executar nenhum.