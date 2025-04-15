
**Data:** 2025-02-12
**keyboards:** 
**links internos:** 
___

# Listas

- **Lista é uma estrutura de dados**:
	- **Homogênea** (Dados do mesmo tipo)
	- **Ordenada** (Elementos acessados por meio de posições)
	- **Inicia vazia**, e seus elementos são alocados sob demanda


- **Tipo (interface): List**
- **Classes que implementam: [[ArrayList]], [[LinkedList]], etc**.

- **Vantagens**:
	- **Tamanho variável**.
	- **Facilidade para se realizar inserções e deleções**.
- **Desvantagens**:
	- **Acesso sequencial aos elementos**.

# Demo 

- Tamanho da list: **size()**
- Obter o elemento de uma posição: **get(position)**
- Inserir elemento a list: **add(obj), add(int, obj)**
- Remover elementos da list: **remove(obj), remove(int), remove(predicate)**
- Encontrar posição de elemento: **indexOf(obj), lastIndexOf(obj)**
- Filtrar List com base em predicado:
	- List< Integer > result = list.stream().filter(x -> x > 4).toList();
- Encontrar primeira ocorrência com base em predicado
	- Integer result = list.stream().filter(x -> x > 4).findFirst().orElse(null);



# Diferenças entre ArrayList e LinkedList

- [[ArrayList]]: É maios rápido quando utilizado para consultar, já para inserção e exclusão, são mais lentas.

- [[LinkedList]]: É mais rápido quando utilizado para inclusão e exclusão de dados com um grande volume de dados. Também pode ser utilizado como [[Queue - Filas]].

