
**Data:** 2024-10-07
**keyboards:** 
**links internos:** 
___

# O que é amarração (ou "binding")?

Em python, amarração ou "binding" refere-se ao processo de associar um nome (identificador)
a um objeto na memória. Essa associação permite que você acesse e manipule o objeto usando o nome atribuído a ele.

## 1. Nomes e objetos

### Nomes: 
São identificadores que você usa em seu código, como nomes de variáveis, funções, classes, etc. Eles são como rótulos que você coloca nos objetos para poder se referir a eles.
### Objetos:
São as entidades que residem na memória do computador e armazenam os dados. Cada objeto possui um tipo (inteiro, string, lista, etc.), um valor e uma indentidade única.

## 2. O processo de amarração (binding)

Quando você cria uma variável e atribui um valor a ela, o Python realiza os seguintes passos:

### Criação do objeto: 
Primeiro, o objeto que representa o valor é criado na memória. Por exemplo, se você atribui o valor 10 à variável ==idade==, um objeto do tipo inteiro com o valor 10 é criado
### Amarração: 
Em seguida, o nome ==idade== é ligado ao objeto recém criado. A partir desse momento, o nome idade se torna uma referência para o objeto 10 na memória.

## 3. Tipos de amarração (binding)

Existem diferentes tipos de amarração em python, dependendo do momento em que a associação entre o nome e o objeto ocorre:

### Amarração em tempo de compilação:
Em algumas linguagens, a amarração ocorre durante a compilação do código. Python, sendo uma linguagem interpretada, não possui esse tipo de amarração.

### Amarração em tempo de execução: 
Em Python, a amarração ocorre em tempo de execução, ou seja, durante a execução do programa. Isso significa que o nome pode ser ligado a diferentes objetos em momentos diferentes.

## 4. Amarração e mutabilidade:

É fundamental entender a relação entre amarração e mutabilidade de objetos:

### Objetos imutáveis:
Quando um nome está ligado a um objeto imutável (como inteiros, strings, e tuplas), qualquer tentativa de modificar o valor do objeto resulta na criação de um novo objeto na memória. O nome é então religado ao novo objeto.
### Objetos mutáveis: 
Quando um nome está ligado a um objeto mutável (como listas e dicionários), você pode modificar o objeto diretamente, sem que um novo objeto seja criado. As alterações feitas no objeto serão refletidas em todas as referências a ele.
#### Exemplo: 
		a = [1, 2, 3]   # 'a' é ligado à lista [1, 2, 3] 
		b = a                      # 'b' agora também se refere à mesma lista 
		b.append(4)           # Modificamos a lista através de 'b' 
		print(a)                   # Saída: [1, 2, 3, 4] - 'a' também reflete a mudança

## 5. [[Escopo]] de amarração

O escopo de um nome define a região do código onde esse nome é válido e pode ser acessado. Python possui diferentes escopos, como escopo global, escopo local de funções e escopo de classes.