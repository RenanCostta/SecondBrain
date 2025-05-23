
**Data:** 2025-03-25
**keyboards:** 
**links internos:** 
___

# Exceções:

- Uma exceção é qualquer condição de erro ou comportamento inesperado encontrado por um programa em **execução**.

- Em Java, uma exceção é um objeto herdado da classe:
	- java.lang.Exception - o compilador obrigada a tratar ou propagar
	- java.lang.RuntimeException - o compilador não obriga a tratar ou propagar

- Quando lançada, uma exceção é propagada na pilha de chamada de métodos em execução, até que seja capturada (tratada) ou o programa seja encerrado


# Hierarquia de exceções do Java:

![[Pasted image 20250325121009.png]]

# Por que exceções?

- O modelo de tratamento de exceções permite que erros sejam tratados de forma consistente e flexível, usando boas práticas

- Vantagens: 
	
	- Delega a lógica do erro para a classe responsável por conhecer as regras que podem ocasionar o erro
	
	- Trata de forma organizada (inclusive hierárquica) exceções de tipos diferentes
	
	- A exceção pode carregar dados quaisquer