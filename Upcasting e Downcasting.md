
**Data:** 2025-03-11
**keyboards:** 
**links internos:** 
___

# Upcasting

**O que é**: É a conversão de um objeto de uma subclasse para um objeto de sua superclasse. 
Essa conversão é sempre segura e implícita, ou seja, o compilador java faz automaticamente.

**Por que é seguro**: Uma Subclasse "é um" tipo de sua superclasse., Portanto, qualquer objeto da subclasse pode ser tratado como um objeto da superclasse.

**Exemplo**: Imagine uma hierarquia de classes onde "Animal" é a superclasse e "Cachorro" é a subclasse. Um objeto "Cachorro" pode ser atribuído a uma variável Animal sem problemas.

- **Casting da subclasse para Superclasse**.
- Uso comum: Polimorfismo


# Downcasting

**O que é**: É a conversão de um objeto de uma superclasse para um objeto de sua subclasse.
Essa conversão é explícita, ou seja , você precisa usar um operador de cast para instruir o compilador a fazer a conversão.

**Por que é potencialmente perigoso**: Nem todo objeto da superclasse "é um" tipo da subclasse. Se você tentar converter um objeto da superclasse que não é uma instância da subclasse, ocorrerá um erro em tempo de execução (ClassCastException).

**Exemplo**: Usando o mesmo exemplo anterior, se você tiver um objeto "Animal" que na verdade é um "cachorro", você pode converte-lo para "Cachorro" No entanto, se o Objeto "Animal" for realmente um "Gato", a conversão falhará.

**Verificação**: Para evitar o erro de ClassCastException, é importante verificar se o objeto da superclasse é um instância da subclasse antes de fazer o downcasting. Isso pode ser feito usando o operador "instanceof"

- **Casting da superclasse para subclasse**.
- **Palavra instanceof**.
- **Uso comum: Métodos que recebem parâmetros genéricos (Equals)**.


Exemplo: 

![[Pasted image 20250311161406.png]]
