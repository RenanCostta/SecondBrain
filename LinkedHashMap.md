
**Data:** 2025-04-08
**keyboards:** 
**links internos:** 
___

### 🔗 **O que é um LinkedHashMap?**

Um **LinkedHashMap** é uma estrutura de dados que armazena **pares chave-valor**, assim como o `HashMap`, **mas mantém a ordem de inserção dos elementos**.


### 🔧 **Como funciona?**

- Internamente usa uma **tabela hash** (como o `HashMap`) **+ uma lista duplamente ligada** para manter a ordem dos elementos.
    
- Pode manter:
    
    - **Ordem de inserção** (padrão).
        
    - **Ordem de acesso** (opcional, útil para caches tipo LRU)


### ✅ **Vantagens**

- Mantém os dados **ordenados por inserção**.
    
- Acesso rápido como no `HashMap`.
    
- Pode ser usado para **implementações de cache LRU**.


## ⚠️ **Desvantagens**

- Levemente mais lento e consome mais memória que `HashMap` (por causa da lista ligada).
    
- Como o `HashMap`, **permite uma chave nula**, mas só uma.