
**Data:** 2025-02-11
**keyboards:** 
**links internos:** 
___

# Construtor

- É uma operação especial da classe, que executa no momento da instanciação do objeto


- Uso comuns:
	- Iniciar valores dos atributos 
	- Permitir ou obrigar que o Objeto receba dados / dependências no momento de sua instanciação (Injeção de dependência)

- Se um construtor customizado não for especificado, a classe disponibiliza o construtor padrão:
	-  Product p = new Product();

- É possivel especificar mais de um construtor na mesma classe



**Problema Exemplo**:

Quando executamos o comando abaixa, instanciamos um produto "product" com seus atributos "vazios":

![[Pasted image 20250211151254.png]]

Entretanto, faz sentido um produto que não tem nome? Faz sentido um produto que não tem preço?

com o intuito de evitar a existência de produtos sem nomes e sem preço, é possivel fazer com que seja "obrigatória" a iniciação desses valores? 

veja um construtor personalizado abaixo que permite essa ação:


**Código exemplo**:

![[Pasted image 20250211151038.png]]


