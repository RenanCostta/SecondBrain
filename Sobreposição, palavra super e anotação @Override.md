
**Data:** 2025-03-12
**keyboards:** 
**links internos:** 
___

# Sobreposição ou sobescrita

- **É a implementação de um método de uma superclasse na subclasse**.

- **É fortemente recomendável usar a anotação *==@Override==* em um método sobrescrito**.
	- Facilita a leitura e compreensão do código
	- Avisamos ao compilador (Boa prática).


![[Pasted image 20250312094136.png]]


**Resolvemos assim**:

![[Pasted image 20250312094206.png]]



# Palavra super

É possível chamar a implementação da superclasse usando a palavra **super**.

Exemplo: Suponha que, na classe BusinessAccount, a regra para saque seja realizar o saque normalmente da superclasse, e descontar mais 2.0

![[Pasted image 20250312094451.png]]



# Recordando: Usando super em construtores 

![[Pasted image 20250312094534.png]]





