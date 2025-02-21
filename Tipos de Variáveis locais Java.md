___


# Variáveis locais:

- Declaradas dentro de um método, construtor ou bloco de código. 
- Apenas acessíveis dentro do bloco onde foram declaradas
- Devem ser Inicializadas antes do Usos

*Exemplo:*

```
public void meuMetodo() {
    int numero = 10; // variável local
    System.out.println(numero);
}
```


# Variáveis de Instâncias (ou atributos):

- Declaradas dentro de uma classe, mas fora de qualquer método, construtor ou bloco.
- Acessíveis por todos os métodos da classe.
- Recebem valores padrão (0 para números, false para booleanos, null para objetos)

*Exemplo:*

```
public class MinhaClasse {
    int contador; // variável de instância

    public void incrementar() {
        contador++;
    }
}
```



# Variáveis Estáticas (ou de classes):

- Declaradas com palavra-chave ==static==, dentro de uma classe, mas fora de qualquer método, construtor ou bloco.
- Acessíveis por todos os métodos da classe e compartilhadas por todas as Instâncias da classe.
- Recebem valores padrão se não foram inicializadas explicitamente.

*Exemplos:*

```
public class MinhaClasse {
    static int totalInstancias = 0; // variável estática

    public MinhaClasse() {
        totalInstancias++;
    }
}
```



# Resumos das diferenças:

![[Pasted image 20250220190037.png]]
