
**Data:** 2024-10-10
**keyboards:** 
**links internos:** 
___

# Personalizando Seletores

Para começar a dar mais poder a CSS, criando estilos personalizados,
precisamos aprender a utilizar seletores de **id** (#) e **class** (.) de maneira
eficiente. Ao criar nosso conteúdo em HTML, podemos **identificar** um
determinado elemento único com um ==id==, ou agrupar elementos
múltiplos que tenham características semelhantes com um ==class==. Vamos
olhar olhar um exemplo simples de documento HTML, 
com propriedades identificadoras:

![[Captura de tela 2024-10-10 195134.jpg]]

Olhando atentamente para a **linha 23**, vimos que o < h1 > se diferencia
dos demais que estão nas **linhas 24 e 27**, pois ele possui um ==id==.

Agora foque sua atenção nas **linhas 25 e 28** e perceba que os dois 
títulos < h2 > possuem o mesmo ==class==.

Um ==id== vai **identificar** um elemento único dentro da página atual.
Essa identificação vai nos permitir criar um estilo especial para um
elemento isolado. Já um ==class== vai identificar uma **classe** à qual um ou 
mais elementos pertençam, compartilhando características em comum
a todos os que façam parte desse grupo

![[Captura de tela 2024-10-10 200022.jpg]]


Em seguida, baseado no código HTML visto anteriormente, vamos criar um estilo local criando uma área < style > dentro da seção < head > do documento atual.

![[Captura de tela 2024-10-10 200216.jpg]]

O que fizemos foi criar configurações simples de estilo baseadas nos elementos *body*, 
h1 e h2 do nosso HTML. Até o momento, não fizemos nenhuma configuração personalizada para nenhum seletor. O resultado é bem previsível:

![[Captura de tela 2024-10-10 200548.jpg]]

Perceba no resultado a cima que os dois primeiros títulos possuem apresentações idênticas, mesmo que o primeiro deles possuem um ==id==.

Isso aconteceu porque não fizemos nenhuma configuração específica para ele. não adianta colocar apenas ==id== ou ==class== em uma elemento e não personalizar o resultado visual usando seletores personalizados.

Agora vamos adicionar algumas declarações e seletores personalizados, ainda dentro da área < style > que criamos:

![[Captura de tela 2024-10-10 200604.jpg]]

No código acima, criamos seletores com simbologias novas. Isso porque não são seletores para elementos HTML, e sim seletores para ==id== e ==class==. Na **linha 21**, criamos um seletor personalizado para o identificador *titulo-principal*, que está atribuído ao h1. Você deve ter percebido que colocamos um símbolo ==#== antes do ==id==.

Já as **linhas 27 e 31** são seletores que receberão declarações para as classes **tópico e texto**.
Todos os seletores personalizados para uma ==class== são identificados por um ponto que vem antes do nome da classe.

![[Captura de tela 2024-10-10 202752.jpg]]


Ao adicionar os seletores personalizados ao nosso estilo local, o resultado fica bem diferente:

![[Captura de tela 2024-10-10 202915.jpg]]

Analise os dois resultados acima e perceba as diferenças. Note que apenas o título h1 identificado como "título-principal" ganhou uma formatação diferente e os demais títulos de mesmo nível se mantiveram como antes.
Inclusive, compare o resultado diferente obtido entre o primeiro e o segundo parágrafos. Apenas o primeiro ficou justificado.
Isso foi por conta da aplicação de uma ==class== apenas ao primeiro (Volte lá no código HTML inicial e confira que o segundo parágrafo não possui uma ==class==).


# Propriedades herdadas

No **capítulo 12**, discutimos três técnicas usadas para aplica estilos aos nossos documentos HTML: **inline**, **local** e **externa**. Durante os nossos vídeos de acompanhamento do material em PDF, demonstramos que as três técnicas podem ser usadas em conjunto, e os estilo de cada serão combinados nessa ordem:

1 lugar: **CSS externo**
2 lugar: **CSS interno/local**
3 lugar: **CSS inline**

Sendo assim, caso haja duplicidade nas configurações, o que fica valendo no final é a propriedade especificada nas configurações inline.
Cada camada de aplicação de estilos vai adicionando propriedade novas e sobrescrevendo as configurações do nível anterior.
Quando nós aplicamos configurações personalizadas de ==id== ou de ==class==, também vai existir uma combinação de configurações, como você já deve ao analisar o exemplo que apresentamos nas páginas anteriores.

voltando ao exemplo dado anteriormente (que vou replicar aqui para facilitar o entendimento) logo no início do corpo, tinhamos dois elementos h1:

![[Captura de tela 2024-10-10 221123.jpg]]

Essas duas configurações de tamanho e cor da fonte serão aplicadas aos dois títulos, já que ambos são do tipo h1. Por fim, adicionamos uma configuração específica para o elemento que tem um ==id== personalizado:

![[Captura de tela 2024-10-10 221337.jpg]]

Dessa maneira, o primeiro h1 do código HTML (aquele que tem um ==id==) ganhará mais três configurações - cor de fundo, cor de fonte e alinhamento de texto - graças a esse seletor extra. Note que na primeira configuração CSS dos elementos h1, dissemos que a cor era *darkgreen*.

Porém, quando aplicamos a segunda configuração de *color* no seletor "#titulo-principal", ele vai sobrescrever o valor da propriedade para White. As outras duas propriedades (background-color e text-align) serão adicionadas às configurações desse primeiro título. O segundo título não sofrerá alterações, já que apenas o primeiro possui o ==id== referido no seletor.


![[Captura de tela 2024-10-10 222725.jpg]]

# Pseudo-classes e pseudo-elementos

Uma pseudo-classe CSS é uma palavra-chave adicionada às declarações de um seletor após um sinal de dois pontos e especificam um estado especial de um elemento.
Existem várias pseudo-classes para estilos, podemos citar ***:hover, :visited, :active, :checked, :empty e :focus.***

Já um pseudo-elemento CSS é uma palavra-chave adicionada às declarações de um seletor após dois sinais de dois pontos e permitem que você formate um pedaço específico do elemento referenciado. 
Os principais pseudo-elementos usados nas CSS são: ***:before, :after, :first-letter, :first-line.***

Vamos começar criando um exemplo bem simples e bastante usado para exemplificar o uso de pseudo-classes e pseudo-elementos: a personalização de links.

![[Captura de tela 2024-10-10 223811.jpg]]

Começando pelo corpo do documento, contendo só o HTML, vamos criar um texto com um título e três parágrafos, com três link. Note que o último link recebeu a atribuição de um classe específica. O resultado esta sendo apresentado a seguir:

![[Captura de tela 2024-10-10 224231.jpg]]

Na imagem acima, o primeiro link apareceu com a cor violeta pois já tínhamos visitado o perfil do GitHub anteriormente. Por padrão, os navegadores mostram links inéditos em azul e os visitados em violeta. Todos os links também aparecem sublinhados por padrão.

Vamos alterar essa apresentação padrão com nossas configurações de estilo. Crie a área < style > dentro de < head > e coloque os seguintes seletores.


![[Captura de tela 2024-10-10 224602.jpg]]

Nas declarações acima, criamos três configurações para os links: a primeira (**linha12**) para os links inéditos (não visitados), colocando o texto em negrito, removendo o sublinhado e colocando-os em cor vermelha.

No segundo seletor para links (**linha 18**), configuramos as âncoras já visitadas (com a pseudo-classe ***:visited***). Nele, apenas mudamos a cor para vermelho escuro.

Já na terceira declaração (**linha 22**), fizemos configurações para todos os links, quando passarmos o mouse por cima (pseudo-classe ***:hover***) e o sublinhado volta a aparecer.

O resultados visual está aparecendo abaixo, compare com o resultado anterior e veja as diferenças: 

![[Captura de tela 2024-10-10 225637.jpg]]

por fim, Vamos adicionar algumas configurações relacionadas à classe especial, criada no documento HTML, ara o terceiro link.

![[Captura de tela 2024-10-10 225813.jpg]]

Na primeira declaração do código acima (**linha 26**), dizemos que o link da classe especial vai ter letra branca, fundo preto e perderá o sublinhado apenas quando movermos o mouse sobre ele.

Nas proximas declarações (**linhas 32 e 37**), vamos adicionar um símbolo >> antes e outro símbolo << depois usando os pseudo-elementos  : :before  e  : :after, respectivamente. O resultado dessas declarações está apresentado a seguir: 

![[Captura de tela 2024-10-10 230658.jpg]]

