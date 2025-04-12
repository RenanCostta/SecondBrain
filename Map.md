
**Data:** 2025-04-08
**keyboards:** 
**links internos:** 
___

# Map<K,V>

É uma coleção de pares **Chave / Valor**.
 - Não permite repetições do objeto chave
 - Os elementos são indexados pelo objeto chave (não possuem posição)
 - Acesso, inserção e remoção de elementos são **Rápidos**.

Uso comum: ***cookies, local storage, qualquer modelo chave-valor***.

Principais implementações:
- **[[HashMap]]** - mias rápido (operações O(1) em tabela hash) e não ordenado.
- **[[TreeMap]]** - mais lento (operações O(log(n) em árvore rubro-negra) e ordenado pelo compareTo do objeto (ou comparator)
- **[[LinkedHashMap]]** - velocidade intermediária e elementos na ordem em que são adicionados