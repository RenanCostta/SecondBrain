
**Data:** 2024-09-30
**keyboards:** 
**links internos:** 
___
# O que é tipagem dinâmica?

Na tipagem dinâmica, o tipo de uma variável é determinado em tempo de execução, em vez de ser definido estaticamente durante a compilação do código. Isso significa que você não precisa declarar explicitamente o tipo de uma variável quando a cria. Python, como linguagem de tipagem dinâmica, permite que você atribua valores de diferentes tipos a uma mesma variável ao longo do tempo.

1. **Criação de variáveis:** você pode simplesmente atribuir um valor a uma variável sem especificar seu tipo:

```x = 10      # x é um inteiro
print(type(x))  # <class 'int'>

x = "Olá"   # agora x é uma string
print(type(x))  # <class 'str'>
```

2. **Mudança de tipo:** você pode mudar o tipo da variável a qualquer momento.

  ```
  x = [1, 2, 3]  # x é uma lista
print(type(x))  # <class 'list'>

x = 3.14      # agora x é um float
print(type(x))  # <class 'float'>

```

3. **Funções e tipos:** Em funções, você pode receber diferentes tipos de argumentos sem se preocupar com a sua tipagem. 

```
def imprime(valor):
	print(valor)

imprime(5)         # imprime um inteiro
imprime("texto")   # imprime uma string
imprime([1, 2, 3]) # imprime uma lista
```

## Vantagens da tipagem dinâmica 

-  **Flexibilidade:** você pode escrever código de forma mais rápida e concisa, sem precisar especificar tipos explicitamente.

- **Programação rápida:** Permite protótipos mais rápidos e desenvolvimento ágil. 

## Desvantagens da tipagem dinâmica 

- **Erros em tempo de execução:** Como os tipos são verificados em tempo de execução, alguns erros só aparecem quando o código é executado. isso pode levar alguns bugs difíceis de detectar.
- **Desempenho:** A tipagem dinâmica pode ser menos eficiente em termos de desempenho, pois o python precisa verificar os tipos de durante a execução
- **Menos Estrutura**: Em projetos maiores, a falta de definição de tipos pode tornar o código mais difícil de entender e manter.

# Conclusão

A tipagem dinâmica é uma característica da linguagem python, oferecendo flexibilidade e facilidade no uso. no entanto, é importe estar ciente de suas desvantagens, especialmente ao trabalhar em projetos maiores, onde a clareza e a manutenção do código são crucias. Em muitos casos, o uso de ferramentas de tipagem estática, como MYPY, pode ajudar a mitigar alguns dos problemas associados á tipagem dinâmica.