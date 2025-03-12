
**Data:** 2025-03-12
**keyboards:** 
**links internos:** 
___

# Classes e métodos final

- Palavra chave: **final**

- **Classe**: Evita que a classe seja herdada

	public final class SavingsAccoutn {
	}

- **Método**: evita que o método sob seja sobreposto.

![[Pasted image 20250312101938.png]]




# Exemplo - método final

Suponha que você não queira que o método withDraw de SavingsAccount seja sobreposto

![[Pasted image 20250312102139.png]]




# Pra quê?

- **Segurança**: Dependendo das regras do negócio, às vezes é desejável garantir que uma classe não seja herdada, ou que um método não seja sobreposto.
	- Geralmente convém acrescentar **final** em métodos sobrepostos, pois sobreposições múltiplas pode ser uma porta de entrada para inconsistências

- **Performance**: atributos de tipo de uma classe final são analisados de forma mais rápida em tempo de execução
	- Exemplo clássico: Classe String.
