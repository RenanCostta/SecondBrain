
**Data:** 2025-02-11
**keyboards:** 
**links internos:** 
___

# Membros estáticos

- Também chamados de Membros de classe
	- Em oposição a membros e instâncias


- São membros que fazem sentido independentemente de Objetos. Não precisam de objeto para serem chamados. São chamados a partir do próprio nome da classe.

- **Aplicações comuns**:
	- Classes utilitárias (math.sqrt(double))
	- Declaração de constantes

- Uma classe que possui apenas membros estáticos, pode ser uma classe estática também. Esta classe não poderá ser instanciada.

![[Pasted image 20250211135413.png]]

**Contexto**:

- Métodos estáticos não podem acessar variáveis de instância (Não estática) diretamente, pois não tem acesso ao contexto de um objeto específico.
- No entanto, métodos estáticos podem acessar variáveis de classe (estáticas) e outros métodos estáticos.


**Tipos de membros estáticos:**

- **Variáveis estáticas (Variáveis de classe)**:
	- São usadas armazenar valores que são compartilhados por todos os objetos da classe.
	- Úteis para constantes, contadores ou valores que precisam ser acessados globalmente pela classe

- **Métodos estáticos**:
	- São usados para realizar operações que não dependem do estado de um objeto específico.
	- Úteis para métodos utilitários, cálculos matemáticos ou operações que manipulam apenas variáveis estáticas.
	- O método main é um método estático, e por causa disso a JVM (máquina virtual do java) consegue executá-lo sem instanciar um objeto.

- **Blocos estáticos**:
	- São blocos de código que são executados apenas um vez, quando a classe é carregada na memória.
	- Úteis para inicializar variáveis estáticas ou realizar operações de inicialização da classe.



**Quando usar Membros estáticos**:

- Quando você precisa de um valor ou método que seja compartilhado por todos os objetos da classe.
- Quando você precisa de um método utilitário que não dependa do estado de um objeto específico.
- Quando se precisa de uma constante que pode ser acessada de qualquer lugar da aplicação.


Membros estáticos são uma ferramenta poderosa em Java, permitindo criar código mais eficiente e organizado.