
**Data:** 2025-04-01
**keyboards:** 
**links internos:** 
___

Gulp é uma ferramenta de automação de tarefas (task runner) baseada em JavaScript, que utiliza Node.js como plataforma. Ele foi projetado para simplificar e agilizar processos repetitivos no desenvolvimento web, como minificação de arquivos, compilação de pré-processadores (como Sass ou Less), otimização de imagens, recarregamento automático do navegador (live reload) e muito mais. O Gulp é conhecido por sua abordagem baseada em "fluxo" (streams) e por ser altamente configurável.

### Como funciona:

O Gulp utiliza um arquivo chamado gulpfile.js, onde você define tarefas (tasks) usando JavaScript. Ele trabalha com o conceito de "pipes", que permite encadear operações de forma eficiente, processando arquivos em memória antes de gravá-los no disco.

### Principais características:

1. **Streams**: Processa arquivos em fluxo, o que torna a execução mais rápida em comparação com ferramentas que gravam arquivos intermediários.
2. **Plugins**: Possui um ecossistema rico com centenas de plugins para tarefas como compressão de CSS/JS, concatenação de arquivos, linting, entre outros.
3. **Código sobre configuração**: Diferente de ferramentas como Grunt (que usa JSON), o Gulp permite escrever lógica em JavaScript, oferecendo mais flexibilidade.
4. **Automação**: Ideal para workflows de desenvolvimento, como compilar código, testar e preparar builds para produção.

### Vantagens:

- **Velocidade**: Por usar streams, evita a criação de arquivos temporários desnecessários.
- **Simplicidade**: A sintaxe é clara e direta, especialmente para quem já conhece JavaScript.
- **Flexibilidade**: Pode ser adaptado para praticamente qualquer necessidade de automação.