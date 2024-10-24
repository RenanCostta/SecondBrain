
**Autor:** 
**Data:** 
**Keywords:** 
**link internos:** 
___
# Exercícios do cap. 1.1

## 1.1-1

***Cite um exemplo real que exija ordenação ou um exemplo real que exija o cálculo de uma envoltória convexa***?

**R**: 
- **Busca na web**: Quando você pesquisa algo no Google, os resultados são ordenados por relevância. Essa ordenação é feita por algoritmos complexos que levam em conta diversos, fatores, como a qualidade do conteúdo, a popularidade do site e a sua localização.
- **Compras online**: Sites de comércio eletrônico usam algoritmos de ordenação para mostrar os produtos mais relevantes pra você, com base em suas pesquisas anteriores, compras e avaliações.

## 1.1-2

***Além da velocidade, que outras medidas de eficiência poderiam ser usadas em uma configuração real?***

**R:**
- ***Uso de recursos:***
	- **Memória**: a quantidade de memória RAM utilizada pelo programa. 
	- **CPU**: que indica o quanto o processador está sendo exigido pelo programa, porque um alto uso de CPU pode causar lentidão no sistema.
	- **energia**: a quantidade de energia consumida pelo programa é um fator importante em dispositivos móveis e sistemas que precisam operar por longos períodos com a bateria.
	- **Largura de banda**: Em aplicações que envolvem transferência de dados pela rede, a quantidade de largura de banda utilizada é crucial para garantir a performance.

- ***Manutenibilidade:***
	- **Legibilidade**: Um código legível e bem documentado é mais fácil de entender, modificar e manter.
	- **Modularidade**: Dividir o código em módulos menores e independentes facilita a reutilização, o teste e a manutenção.
	- **Extensibilidade**: Um código extensível é aquele que pode ser facilmente adaptado para novas funcionalidades ou requisitos.


## 1.1-3

***Selecione uma estrutura de dados que você já tenha visto antes e discuta seus pontos fortes e suas limitações.***:

**R**:
Falarei sobre a estrutura de dados **Fila**..

***Pontos fortes***: 

- **Simples de entender e implementar**: A fila segue o modelo FIFO (first-in, first-out), o que a torna mais fácil de compreender e implementar código.
- **eficiente para gerenciar código**: Ideal para situações onde a ordem de chegada é crucial, como em filas de impressão, gerenciamento de tarefas em sistemas operacionais ou processamento de eventos em jogos.
- **Baixo overhead**: A fila geralmente tem um baixo overhead de memória, pois armazena apenas os elementos e ponteiros para o próximos elemento.

***Limitações***:

- **Acesso restrito**: Só é possível acessar o primeiro elemento da fila (o mais antigo). Para acessar outros elementos, é necessário remover os elementos anteriores.
- **Ineficiente para buscas**: A fila não é projetada para buscas eficientes. Encontrar um elemento específico pode exigir a remoção de vários elementos até encontra-lo.


## 1.1-4

***Em que aspectos os problemas anteriores do caminho mais curto e do caixeiro-viajante são semelhantes? Em que aspectos eles são diferentes?***

**R:**
O problema do caminho mais curto e o problema do caixeiro-viajante (PCV) são problemas clássicos na ciência da computação, com aplicações em diversas áreas como logísticas, planejamento de rotas e redes de computadores. Apesar de parecerem semelhantes à primeira vista, eles possuem diferenças importantes em seus objetivos e complexidade.


***Semelhança**:

- **Grafos**: Ambos os problemas são definido em grafos, onde os nós representam locais (cidade, cruzamentos, etc.)
- **Caminhos**: Ambos os problemas buscam encontrar um caminho entre nós no grafo, minimizando o custo total (distância, tempo, etc.) associado ao caminho.
- **Otimização**: Ambos são problemas de otimização, buscando a melhor solução dentre um conjunto de soluções possíveis.

***Diferenças***:

- **Objetivos**: 
	- **O caminho mais curto**: Existem algoritmos eficientes com complexidade polinomial para resolver o problema do caminho mais curto, como o algoritmo de ==dijkstra==.
	- **Caixeiro-viajante**: É um problema NP-difícil, oq eu significa que não existe algoritmo conhecido que o resolva em tempo polinomial para todos os casos. A complexidade aumenta exponencialmente como o número de nós.
- **Abordagens de solução:** 
	 - **O caminho mais curto**: Algoritmos como ==dijkstra== e ==Bellman-Ford== são amplamente utilizados. 
	 - **Caixeiro-viajante**: Devido à sua complexidade, são utilizadas heurísticas e algoritmos de aproximação para encontrar soluções próximas do ótimo tempo razoável. Exemplos incluem algoritmos genéticos, ==simulated annealing== e ==branch and bound==.


***Em resumo:***

Embora ambos os problemas envolvam encontrar caminhos em grafos, problema do caixeiro viajante é consideravelmente mais complexo do que o problema do caminho mais curto.
A necessidade de visitar todos os nós e retornar ao ponto de partida torna o PCV um desafio computacional significativo, com implicações importantes para diversas áreas de aplicação.



## 1.1-5

