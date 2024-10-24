
**Data:** 2024-10-11
**keyboards:** 
**links internos:** 
___

# JavaScript tem 7 tipos primitivos:

1. **String:** Representa texto. Sempre entre aspas simples (`' '`) ou duplas (`" "`).
    
    - Ex: `"Olá, mundo!"`, `'JavaScript'`.
2. **Number:** Representa números, tanto inteiros quanto decimais.
    
    - Ex: `10`, `3.14`, `-5`.
3. **Boolean:** Representa um valor lógico, que pode ser `true` (verdadeiro) ou `false` (falso).
    
    - Ex: `true`, `false`.
4. **Null:** Representa a ausência intencional de um valor.
    
    - Ex: `null`.
5. **Undefined:** Indica que uma variável foi declarada, mas ainda não recebeu um valor.
    
    - Ex: `let nome;` (a variável `nome` está `undefined`).
6. **Symbol:** Introduzido no ES6, cria valores únicos e imutáveis, úteis para identificar propriedades de objetos.
    
    - Ex: `Symbol('descricao')`.
7. **BigInt:** Permite representar números inteiros maiores do que o limite permitido por `Number`. Útil para cálculos de alta precisão.
    
    - Ex: `123456789012345678901234567890n`.

## Exemplos:

```
let nome = "Maria";      // String
let idade = 30;          // Number
let ehMaiorDeIdade = true; // Boolean
let cidade = null;        // Null
let profissao;           // Undefined (não foi atribuído valor)
```

## Observações importantes:

- **Tipagem dinâmica:** JavaScript tem tipagem dinâmica, o que significa que o tipo de uma variável é determinado pelo valor que ela armazena, e esse tipo pode mudar durante a execução do código.
- **Imutabilidade:** Os tipos primitivos são imutáveis. Isso significa que, uma vez criado um valor primitivo, ele não pode ser alterado.

Entender variáveis e tipos primitivos é fundamental para começar a programar em JavaScript. Com este conhecimento, você poderá armazenar e manipular informações de forma eficiente em seus programas.