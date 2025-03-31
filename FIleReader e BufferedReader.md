
**Data:** 2025-03-31
**keyboards:** 
**links internos:** 
___

# Classes:

- **FileReader** - (stream de leitura de caracteres a partir de arquivos)
	• https://docs.oracle.com/javase/10/docs/api/java/io/FileReader.html

- **BufferedReader** - (Mais rápido)

# Diferenças entre os dois:


#### **FileReader**:

- É uma classe da API de entrada/saída (java.io) projetada para ler fluxos de caracteres diretamente de um arquivo.
- Funciona como um leitor de baixo nível, acessando o arquivo caractere por caractere ou em blocos pequenos, dependendo do sistema operacional.
- Não possui mecanismo interno de buffer, o que significa que cada chamada de leitura vai diretamente ao sistema de arquivos.


#### **BufferedReader**:

- É uma classe que encapsula um Reader (como o FileReader) e adiciona um buffer para reduzir o acesso direto ao recurso subjacente (como o arquivo).
- Seu propósito principal é melhorar o desempenho ao ler grandes quantidades de dados, minimizando chamadas ao sistema operacional.


# Relacionamento entre as duas:

- BufferedReader não substitui FileReader, mas o complementa. O FileReader é frequentemente passado como argumento ao construtor do BufferedReader para fornecer o fluxo de caracteres que será bufferizado.

- Em outras palavras, o BufferedReader é uma camada de abstração mais alta que melhora a eficiência do FileReader.
