
**Data:** 2024-05-22
**keyboards:** #html #semântica 
**links internos:** 
___
# Semântica

A maior mudança da HTML4 para a HTML5 é o acréscimo da semântica aos elementos.

No dicionário Michaelis: 

	Semântica é o significado dos vocábulos, por oposição a sua forma.

Analisando a frase acima percebemos que uma palavra pode ter **forma** e **significado**, e que a **semântica** dá mais valor ao significado.

Na HTML4, tínhamos tags como < b > que colocava um texto em negrito,
< u > que colocava o termo sublinhado e < blink > que fazia o texto piscar.
Essas eram tags que representavam apenas uma **forma**. Você dizia que queria um texto sublinhado, mas qual era o motivo? Qual era o sentido de sublinhar alguma coisa? Vamos ver um exemplo:

	Juvenal era um sujeito de muita sorte. e já começou de pequeno.  onde morou na < u >rua marquês de lira filho </u>. um local de fácil acesso ao centro da cidade.

Em HTML4 colocamos o par de tags < U > para delimitar o termo "rua marquês de lira". isso seria uma maneira de determinar somente um formato visual para chamar atenção para o endereço onde o cara nasceu. O Sublinhado é apenas uma **forma**, sem **significado** explícito. sublinhamos só pra chamar atenção visualmente.

Já a HTML5 chegou com o conceito de valorizar a semântica, logo suas tags tentam levar um **significado** embutido muito forte. logo, a frase acima ficaria assim:

	Juvenal era um sujeito de muita sorte. E já começou de pequeno onde morou na <address>rua marquês de lira filho</address>. um local de fácil acesso ao centro da cidade.

Note agora, usamos a tag < address > para dar um significado ao destaque que fizemos. estamos chamando atenção para a rua marquês de lira por se tratar do endereço da pessoa. No caso, um navegador de celular pode até sugerir que você veja o mapa do local e trace a rota para chegar lá.
viu? **SIGNIFICADO!**

Sendo assim, em HTML5, vemos de forma bastante evidente a presença do chamado **HTML Semântico** ou **Tags semânticas** ou ainda o **Conteúdo semântico**.
Você quer que um endereço apareça na forma de um texto sublinhado? Use CSS para configurar isso, a HTML serve para dar sentido ao conteúdo. É assim que tudo vai funcionar.

Desde a mudança de versões , a **W3C** - Consórcio responsável por normatizar a HTML - tem dado muito valor por adicionar novas tags que tenham mais significado e a tirar algumas tags que só focam no efeito visual (forma) de apresentação. O intuito é deixar a apresentação gráfica por conta das CSS.