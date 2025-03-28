
**Data:** 2025-03-26
**keyboards:** 
**links internos:** 
___

# Sugestão de pacotes "model"

![[Pasted image 20250326114444.png]]


# Problema exemplo:

Fazer um programa para ler os dados de uma reserva de hotel (número do quarto, data de entrada e data de saída) e mostrar os dados da reserva, inclusive sua duração em dias. Em seguida, ler novas datas de entrada e saída, atualizar a reserva, e mostrar novamente a reserva com os dados atualizados. O programa não deve aceitar dados inválidos para a reserva, conforme as seguintes regras: - Alterações de reserva só podem ocorrer para datas futuras - A data de saída deve ser maior que a data de entrada

## UML:

![[Pasted image 20250326114833.png]]



# Resumo da resolução do problema:


### Solução 1 (muito ruim): Lógica de validação no programa principal

- **Lógica de programação não delegada à classe da reserva**

### Solução 2 (ruim): Método retornando string

- **A semântica da operação é prejudicada**
	- Retornar string não tem nada a ver com atualização de reserva
	- E se a operação tivesse que retornar um String?
- **Ainda não é possivel tratar exceções em construtores
- **Ainda não há auxílio do compilador: o programador deve lembrar de verificar se houve erro**.
- **A lógica fica estruturada em condicionais aninhadas**.

### Solução 3 (boa): Tratamento de exceções com [[try-catch]]

![[Pasted image 20250328124511.png]]




# Resumo do resumo:

### **Cláusula throws**: propaga a exceção ao invés de trata-la

### **Cláusula throw**: lança a exceção / "Corta" o método

### **Exception:** Compilador obriga a tratar

### **RuntimeExcepetion**: compilador não obriga

- O modelo de tratamento de exceções permite que erros sejam tratados de forma consistente e flexível, usando boas práticas 
-  Vantagens: 
-  Lógica delegada 
-  Construtores podem ter tratamento de exceções 
-  Possibilidade de auxílio do compilador (Exception) 
- Código mais simples. Não há aninhamento de condicionais: a qualquer momento que uma exceção for disparada, a execução é interrompida e cai no bloco catch correspondente. 
-  É possível capturar inclusive outras exceções de sistema