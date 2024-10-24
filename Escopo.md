
**Data:** 2024-10-07
**keyboards:** 
**links internos:** 
___

# Escopos em Python 

Em python, o escopo de uma variável define a região do código onde ela pode ser acessada e utilizada. Imagine como se cada variável vivesse e um "Bairro" específico dentro do seu código, e esse bairro é o seu escopo.

## Por que entender escopos é crucial?

### Organização: 
Escopos ajudam a organizar o código, evitando conflitos entre variáveis com o mesmo nome em diferentes partes do programa.
### Manutenção:
Códigos com escopos bem definidos são mais fáceis de entender, depurar e modificar, especialmente em projetos grandes.
### Segurança: 
Escopos protegem a variáveis de alterações acidentais em outras partes do código, garantindo a integridade dos dados.


## Tipos de escopos

### Escopo local e variáveis locais

- Variáveis definidas dentro de uma função tem escopo local.
- Só podem ser acessadas dentro dessa função.
###### Exemplo:

```
def minha_funcao():
    x = 10  # x tem escopo local
    print(x)

minha_funcao()  # Saída: 10
print(x)  # Erro! x não é acessível aqui
```

### Escopo Enclosing (não-local) e variáveis não-locais

- Ocorro em função aninhadas.
- A função interna tem acesso às variáveis da função externa

###### Exemplo:

```
def funcao_externa():
    y = 20

    def funcao_interna():
        print(y)  # y é acessível aqui

    funcao_interna()

funcao_externa()  # Saída: 20
```

### Escopo Global e variáveis globais

- Variáveis definidas fora de qualquer função.
- Acessíveis em qualquer parte do código.
###### Exemplo:

```
z = 30  # z tem escopo global

def minha_funcao():
    print(z)

minha_funcao()  # Saída: 30
print(z)  # Saída: 30
```


### Escopo Built-in

- Contém funções e constantes pré-definidas em Python
- Sempre acessíveis.
###### Exemplo:

```
print()
len()
int()
```



## A regra LEGB: O guia definitivo para escopos

Python segue a regra LEGB para determinar o escopo de uma variável. Essa regra define a ordem de busca que o interpretador Python utiliza para encontrar uma variável.

### Local:
Começa no escopo local, ou seja, dentro da função onde a variável é utilizada.

### Enclosing function locals:  
Se não encontrar localmente, busca em funções que englobam a função atual (em caso de função aninhadas).

### Global
Em seguida, procura no escopo global, que abrange todo o arquivo do código.

### Built-in
Por ultimo, busca em escopos pré-definidos da linguagem python, que contêm funções e constantes embutidas (como ==print==, ==len==, etc.)



## Modificando variáveis globais dentro de funções

- Para modificar uma variável global dentro de uma função, utilize a palavra-chave ==global==, como se estivesse solicitando permissão para modificar um monumento da cidade.

###### Exemplo:





