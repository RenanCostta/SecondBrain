
**Data:** 2025-02-12
**keyboards:** 
**links internos:** 
___

# Garbage collector


- **É um processo que automatiza o gerenciamento de memória de um programa em execução**

- **O garbage collector monitora os objetos alocados dinamicamente pelo programa (no heap), desalocando aqueles que não estão mais sendo utilizados.** 


*exemplos:*

![[Pasted image 20250212130522.png]]

![[Pasted image 20250212130540.png]]



# Desalocação por Escopo

![[Pasted image 20250212130641.png]]
![[Pasted image 20250212130650.png]]
![[Pasted image 20250212130708.png]]


# Resumo 

- **Objetos alocados dinamicamente, quando não possuem mais referência para eles, serão desalocados pelo garbage collector.** 

- **Variáveis locais serão desalocadas imediatamente assim que seu escopo local sai de execução.** 

