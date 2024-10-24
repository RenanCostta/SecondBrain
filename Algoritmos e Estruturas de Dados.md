
**Data:** 2024-10-02
**keyboards:** 
**links internos:** 
___

# Introdução

Esta parte o fará refletir sobre o projeto e a análise de algoritmos. Ela foi planejada para ser uma introdução suave ao modo como especificamos algoritmos, a algumas das estratégias de projeto que usaremos ao longo deste livro e a muitas das ideias fundamentais empregadas na análise de algoritmos. As partes posteriores deste livro serão elaboradas sobre essa base. 

## Capítulo 1

O Capítulo 1 é uma visão geral de algoritmos e de seu lugar em modernos sistemas de computação. Esse capítulo define o que é um algoritmo e dá uma lista com alguns exemplos. Além disso, traz a tese de que devemos considerar algoritmos como uma tecnologia, lado a lado com hardware rápido, interfaces gráficas do usuário, sistemas orientados a objetos e redes. 

## Capítulo 2

No Capítulo 2, veremos nossos primeiros algoritmos, que resolvem o problema de ordenar uma sequência de n números. Eles são escritos em um pseudocódigo que, embora não possa ser traduzido diretamente para nenhuma linguagem de programação convencional, transmite a estrutura do algoritmo com clareza suficiente para que você possa implementá-la na linguagem de sua preferência. Os algoritmos de ordenação que examinamos são a ordenação por inserção, que utiliza uma abordagem incremental, e a ordenação por intercalação, que usa uma técnica recursiva conhecida como “divisão e conquista”. Embora o tempo exigido por esses dois algoritmos aumente com o valor n, a taxa de aumento de cada um é diferente. Determinamos esses tempos de execução no Capítulo 2 e desenvolvemos uma notação útil para expressá-los. 

## Capítulo 3

O Capítulo 3 define com exatidão essa notação, que denominamos notação assintótica. O capítulo começa definindo várias notações assintóticas que utilizamos para limitar os tempos de execução dos algoritmos por cima e por baixo. O restante do Capítulo 3 é primariamente uma apresentação da notação matemática, cuja finalidade é mais a de assegurar que o uso que você faz da notação corresponda à que fazemos neste livro do que lhe ensinar novos conceitos matemáticos. 

## Capítulo 4

O Capítulo 4 examina mais a fundo o método de divisão e conquista apresentado no Capítulo 2. Dá exemplos adicionais de algoritmos de divisão e conquista, incluindo o surpreendente método de Strassen para multiplicação de duas matrizes quadradas. O Capítulo 4 contém métodos para solução de recorrências que são úteis para descrever os tempos de execução de algoritmos recursivos. Uma técnica eficiente é o “método mestre”, que frequentemente usamos para resolver recorrências que surgem dos algoritmos de divisão e conquista. Embora grande parte do Capítulo 4 seja dedicada a demonstrar a correção do método mestre, você pode saltar essa demonstração e ainda assim empregar o método mestre. 

## Capítulo 5

O Capítulo 5 introduz análise probabilística e algoritmos aleatorizados. Normalmente usamos análise probabilística para determinar o tempo de execução de um algoritmo em casos em que, devido à presença de uma distribuição de probabilidades inerente, o tempo de execução pode ser diferente para entradas diferentes do mesmo tamanho. Em alguns casos, consideramos que as entradas obedecem a uma distribuição de probabilidades conhecida, de modo que calculamos o tempo de execução médio para todas as entradas possíveis. Em outros casos, a distribuição de probabilidades não vem das entradas, mas de escolhas aleatórias feitas durante o curso do algoritmo. Um algoritmo cujo comportamento seja determinado não apenas por sua entrada mas também pelos valores produzidos por um gerador de números aleatórios é um algoritmo aleatorizado. Podemos usar algoritmos aleatorizados para impor uma distribuição de probabilidade às entradas — garantindo assim que nenhuma entrada específica sempre cause fraco desempenho — ou mesmo para limitar a taxa de erros de algoritmos que têm permissão para produzir resultados incorretos em base limitada. Os apêndices A-D contêm outro material matemático que você verá que são úteis à medida que ler este livro. É provável que você tenha visto grande parte do material dos apêndices antes de ler este livro (embora as definições e convenções específicas de notação que usamos possam ser diferentes em alguns casos daquelas que você já viu) e, portanto, você deve considerar os apêndices material de referência. Por outro lado, é provável que você ainda não tenha visto a maior parte do material contido na Parte I. Todos os capítulos da Parte I e os apêndices foram escritos com um toque de tutorial





# Capítulo 1: [[O papel dos algoritmos na computação]]

O que são algoritmos? Por que o estudo dos algoritmos vala a pena? Qual é o papel dos algoritmos em relação a outras tecnologias usadas em computadores? Neste capítulo, responderemos essas perguntas.

## 1.1 ALGORITMOS
###### O que são?
Informalmente, um **Algoritmo** é qualquer procedimento computacional bem definido que toma algum valor ou conjunto de valores como **Entrada** e produz algum valor ou conjuntos de valores como **Saída**.
Portanto, um Algoritmo é uma sequência de etapas computacionais que transformam a **entrada** em **saída**.

### Problemas computacionais

Também podemos Considerar um algoritmo como uma ferramenta que resolve um **Problema computacional** especificado.

O enunciado do problema específica em termos gerais a relação desejada entre **Entrada** e **saída**. Por exemplo, poderia ser necessário ordenar uma sequência de números em ordem não decrescente. Esse problema surge com frequência na prática e oferece um solo fértil para a apresentação de muitas técnicas de projeto e ferramentas de análise padronizadas. Vejamos como definir formalmente o **Problema de ordenação**:

**Entrada**: Uma sequência de n números 〈a1 , a2 , ..., an 〉. 
**Saída**: Uma permutação (reordenação) 〈a1 ’ , a2 ’, ..., an ’〉 da sequência de entrada, tal que a1 ’ ≤ a2 ’ ≤ ... ≤ an ’

### Instância de um problema 

Imagina que você tem uma receita de bolo. Essa receita é como um algoritmo, um conjunto de instruções para resolver um problema: **Fazer um bolo**.

Agora imagine que você quer fazer um bolo de chocolate, um de cenoura e um bolo de laranja. Cada um desses bolos é uma **instância** do problema **fazer um bolo**. Eles seguem uma mesma receita (o mesmo algoritmo)
mas usam ingredientes diferente (Dados de entrada diferentes).

No estudo de algoritmos, uma instância de um problema é como uma versão específica desse problema com dados de entrada específicos.

**Exemplos**:

- **problema**: Ordenar uma lista de números.

	- **Instância 1:** ordenar a lista [5, 2, 8, 1, 9]
	- **Instância 2:** Ordenar a lista [10, 5, 2, 8, 1, 9, 4].
- **Problema**: Encontrar o menos caminho entre duas cidades.
	- Instância 1: Encontrar o menor caminho entre porto alegre e recife.
	- **Instância 2:** Encontrar o menor caminho entre rio de janeiro e são Paulo.

Cada instância do problema usa o mesmo algoritmo (a mesma receita, o mesmo conjunto de instruções), mas com dados diferentes (Ingredientes diferentes, cidades diferentes).

Entender o conceito de Instância é importante porque a eficiência de um algoritmo pode variar dependendo da instancia. um algoritmo pode ser rápido para uma instancia e lento para outra, mesmo que seja o mesmo problema.


### Que tipos de problemas são resolvidos por algoritmos?

A ordenação não é de modo algum o único problema computacional para o qual os algoritmos foram desenvolvidos (e é provável que você já tenha suspeitado disso quando viu o tamanho deste livro.). As aplicações práticas de algoritmos estão por toda parte e incluem os exemplos a seguir:

#### Comercio eletrônico 

O comércio eletrônico permite que mercadorias e serviços sejam negociados e trocados eletronicamente e depende do sigilo de informações pessoais, como números de cartões de crédito, senhas e extratos bancários.

Entre as principais tecnologias utilizadas no comércio eletrônico estão a criptografia de chave pública e as assinaturas digitais (estudadas no Capítulo 31), ambas baseadas em algoritmos numéricos e na teoria dos números.

#### Indústrias 

Na indústria e em outros empreendimentos comerciais, muitas vezes é preciso alocar recursos escassos da maneira mais benéfica possível. 

Uma empresa petrolífera talvez deseje saber onde localizar seus poços para maximizar o lucro esperado. 

Um político talvez queira determinar onde gastar dinheiro em publicidade de campanha para maximizar as chances de vencer uma eleição. 

Uma empresa de transporte aéreo poderia querer designar tripulações a voos da forma menos dispendiosa possível, garantindo que cada voo seja atendido e que as regulamentações do governo relativas à escala das tripulações sejam obedecidas. 

Um provedor de serviços da Internet talvez queira definir onde alocar recursos adicionais para servir a seus clientes com mais eficiência. 

Todos esses são exemplos de problemas que podem ser resolvidos com a utilização de programação linear, que estudaremos no Capítulo 29.



### Problemas de difícil identificação

Nem todo problema resolvido por algoritmos tem um conjunto de soluções candidatas fáceis de identificar. Por exemplo, suponha que temos um conjunto de valores numéricos que representam amostras de um sinal e que queremos calcular a transformada discreta de Fourier dessas amostras.

A transformada discreta de Fourier converte o domínio do tempo para o domínio da frequência, produzindo um conjunto de coeficientes numéricos, de modo que podemos determinar a força de várias frequências no sinal amostrado. Além de estarem no cerne do processamento de sinais, as transformadas discretas de Fourier também se aplicam a compressão de dados e à multiplicação de grandes polinômios e inteiros. O capítulo 30 apresenta um algoritmo eficiente para esse problema, a transformada rápida de Fourier (comumente chamada de **FFT**), e também apresenta o esquema de projeto de um circuito de *hardware* para calcular a **FFT**.


### Estruturas de dados

Este livro também contém várias estruturas de dados. Uma ***Estrutura de dados*** é um modo de armazenar e organizar dados com o objetivo de facilitar acesso e modificações. Nenhuma estrutura de dados única funciona bem para todas as finalidades e, por isso, é importante conhecer os pontos fortes e as limitações de várias delas.

### Técnica

Embora você possa usar este livro como um "livro de receitas" para algoritmos, é possível que algum dia encontre um problema cujo algoritmo publicado (muito dos exercícios e problemas deste livro, por exemplo) não consiga achar imediatamente. Este livro lhe ensinará técnicas de projeto e análise de algoritmos para que você possa desenvolver algoritmos por conta própria, mostrar que eles fornecem a respostas correta e entender a sua eficiência.

Capítulos diferentes abordam diferentes aspectos da solução de problemas de algoritmos. Alguns abordam problemas específicos: 

como determinar medianas e ordenar dados estatísticos, no capítulo 9.

calcular arvores geradoras (***spanning trees***) mínimas, no capítulo 23. 

e determinar um fluxo máximo em uma rede , no capítulo 26.


Outros capítulos abordam técnicas como a de:

divisão e conquista, no capítulo 4.

programação dinâmica, no capitulo 15.

e análise amortizada, no capitulo 17.


### Problemas difíceis

A maior parte deste livro trata de algoritmos eficientes. Nossa medida habitual de eficiência é a velocidade, isto é, quanto tempo um algoritmos demora para reproduzir seu resultado.
Porém, existem alguns problemas para os quais não se conhece nenhuma solução eficiente. 
O capitulo 34 estuda um subconjunto interessante desses problemas, conhecido como **NP-completos**.

Por que os problemas **NP-completos** são interessantes?

Em primeiro lugar, embora nenhum algoritmo eficiente para um problema **NP-completo** tenha sido encontrado até agora, ninguém jamais provou que não é possível existir um algoritmos eficiente para tal problema. Em outras palavras, Ninguém sabe se existem ou não algoritmos eficientes para problemas **NP-completos**. 

Em segundo lugar, o conjunto de problemas **NP-completos** tem a propriedade notável de que, se existir um algoritmos eficiente para qualquer um deles, então existem algoritmos para todos eles. Essa relação entre os problemas **NP-completos** são semelhantes mas não idênticos a problemas para os quais sabemos existir algoritmos eficientes. cientistas da computação ficam intrigados com o fato de que uma pequena mudança no enunciado do problemas pode provocar uma grande alteração na eficiência do melhor algoritmos conhecido.

É bom que você conheça os problemas **NP-completos** porque alguns deles surgem com frequência surpreendente em aplicações reais. Se você tiver de reproduzir um algoritmos eficiente para um problema **NP-completo**, é provável que perca muito tempo em uma busca infrutífera. Por outro lado, se você conseguir mostrar que o problema é **NP-completo**, poderá dedicar seu tempo ao desenvolvimento de um algoritmo eficiente que ofereça uma solução boa, embora não a melhor possível.

Como exemplo concreto, considere uma empresa transportadora que tenha um depósito central. Todo dia, cada caminhão é carregado no depósito e enviado a diversos locais para fazer entregas. No final do dia, cada caminhão tem de estar de volta ao depósito para ser preparado para a carga do dia seguinte. Para reduzir custos, a empresa  quer selecionar uma ordem de pontos de entrega que represente a menor distância total a ser percorrida por cada caminhão. Esse problema é o famoso "Problema do caixeiro viajante", e é **NP-completo** -- embora não tem nenhum algoritmo eficiente conhecido. Contudo, adotando-se certas premissas, há algoritmos eficientes que fornecem uma distância total não muito acima do menor possível. O capítulo 35 discute esses "algoritmos de aproximação".



### Paralelismo 

Durante muitos anos pudemos contar com uma taxa regular de aumento da velocidade de relógios dos processadores. Porém, limitações físicas representam um entrave fundamental ao crescimento constante dessas velocidades: como a densidade de potência aumenta super linearmente com a velocidade do relógio, existe o risco de derretimento dos chips quando essas velocidades atingem um certo nível.
Portanto, para executar mais cálculos por segundo, o projeto moderno de chips prevê não apenas um, mas vários "núcleos" de processamento. 
Podemos comparar esses computadores com vários núcleos a vários computadores sequenciais em um único chip; em outras palavras, eles são um tipo de "computador paralelo".

Para obter o melhor desempenho desses processadores com vários núcleos, precisamos introduzir algoritmos que consideram o paralelismo. O **Capítulo 27** apresenta um modelo de algoritmo "multithread" que tira proveito de núcleos múltiplos.
Do ponto de vista teórico, esse modelo é vantajoso e constitui a base de vários modelos eficiente de programas de computador, entre eles, um programa para campeonatos de xadrez.


## [[Exercícios 1.1]] 
*aqui tem exercícios do que vimos do assunto do cap. 1.1* 

## 1.2 ALGORITMOS COMO TECNOLOGIA

###### E se os computadores fossem infinitamente rápidos...

Suponha que os computadores fossem infinitamente rápidos e que a memória do computador fosse gratuita. Você teria alguma razão para estudar algoritmos? A resposta é sim, ainda que apenas porque você gostaria de demonstrar que seu método de solução termina, e o faz com a resposta correta. Se os computadores fossem infinitamente rápidos, qualquer método correto para resolver um problema serviria. É provável que você quisesse que sua implementação estivesse dentro dos limites da boa prática de engenharia de software (isto é, que ela fosse bem documentada e projetada) mas, na maior parte das vezes, você utilizaria o método que fosse mais fácil de implementar. É claro que os computadores podem ser rápidos, mas eles não são infinitamente rápidos. A memória pode ser de baixo custo, mas não é gratuita. Assim, o tempo de computação é um recurso limitado, bem como o espaço na memória. Esses recursos devem ser usados com sensatez, e algoritmos eficientes em termos de tempo ou espaço o ajudarão a usá-los assim.



### Eficiência:

Algoritmos diferentes criados para resolver o mesmo problema muitas vezes são muito diferentes em termos de eficiência. Essas diferenças podem ser muito mais significativas que as diferenças a hardware e software.

Como no exemplo no capítulo 2, estudaremos dois algoritmos de ordenação. O primeiro conhecido como ***Ordenação por inserção***, leva um tempo aproximadamente proporcional a: $c_1n^2$ para ordenar *n* itens, onde $c_1$ é uma constante que não depende de $n$. Isto é, ele demora um tempo aproximadamente proporcional a $n_2$. 
O segundo, conhecido por ***Ordenação por intercalação***, isso leva um tempo aproximadamente igual a $c_2n$ $lg$ $n$, onde $lg$ $n$ representa $log^2$ $n$ e $c_2$ é outra constante que também não depende de $n$. A ordenação por inserção normalmente tem um fator constante menor que a ordenação por intercalação; assim $c_1$ < $c_2$. veremos que os fatores constantes pode causar um impacto muito menor sobre o tempo de execução que a dependência do tamanho de entrada $n$. Se representarmos o tempo de execução da ordenação por inserção por $c_1n.n$ e o tempo de execução da ordenação por intercalação por $c_2n.lgn$, veremos que, enquanto o fator tempo de execução da ordenação por inserção é $n$, o da ordenação por intercalação é $lgn$, que é muito menor (por exemplo, quando n = 1.000, $lg$ $n$ é aproximadamente 10 e quando $n$ é igual a um milhão, $lg$ $n$ é, aproximadamente só 20). Embora a ordenação por inserção em geral seja mais rápida que a ordenação por intercalação para pequenos tamanhos de entradas, tão logo o tamanho da entrada $n$ se torne grande o suficiente a vantagem da ordenação por intercalação de $lg$ $n$ contra $n$ compensará com sobras a diferença entra fatores constantes. Independentemente do quanto $c_1$ seja menor que $c_2$, sempre haverá um ponto de corte além do qual ordenação por intercalação será mais rápida.


