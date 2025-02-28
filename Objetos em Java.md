
**Data:** 2025-02-28
**keyboards:** 
**links internos:** 
___

# O que é um Objetos?

**Objetos São a Chave para entender a tecnologia de orientada a Objetos. Olhe ao redor agora mesmo e você encontrará muitos exemplos de objetos no mundo real. Seu cachorro, sua mesa, seu aparelho de televisão, sua bicicleta**...

**Objetos do mundo real compartilham duas características: todos eles tem estado (state) e e comportamento (behavior) cachorros tem state (nome, cor, raça, fome) e comportamento (latindo, buscando e abanando o rabo). Bicicletas também tem state (marcha atual, cadência atual do pedal, velocidade atual) e comportamento (trocando marcha, trocando cadencia do pedal, aplicando freios). Identificar o estado e o comportamento de objetos no mundo real é uma ótima maneira de começar a pensar em termos de programação orientada a objetos**.

**Para cada objeto que você vê, faça a si mesmo duas perguntas: "Em quais estados possíveis esse objeto pode estar?" e "Qual comportamento possível esse objeto pode executar?". Certifique-se de anotar suas observações. Ao fazer isso, você notará que os objetos do mundo real variam em complexidade; sua luminária pode ter apenas dois estados possíveis (ligado e desligado) dois comportamentos possíveis (ligar e desligar), mas seu rádio de mesa pode ter estados adicionais (ligado, desligado, volume atual, estação atual) e comportamento (ligar, desligar, aumentar volume, diminuir volume, escanear, sintonizar). Você também pode notar que alguns objetos, por sua vez, também conterão outros objetos. Todas essas observação do mundo Real se traduzem no munda da programação orientada a objetos**.

![[Pasted image 20250228090227.png]]

**Objetos de software são conceitualmente similares a objetos do mundo real: eles também consistem em estado e comportamento relacionado. Um objeto armazena seu estado em *Campos* (variáveis em algumas linguagens de programação). e expões seu comportamento por meio de métodos (funções em algumas linguagens de programação). Os métodos operam no estado interno de um objeto e servem como o mecanismo primário para comunicação objeto a objeto. Ocultar o estado interno e exigir que toda a interação seja realizada por meio de um objeto é conhecido como *Encapsulamento de dados* -- um princípio fundamental da programação orientada a objetos**.


considere uma bicicleta, por exemplo:

![[Pasted image 20250228092739.png]]


**Ao atribuir estado (velocidade atual, cadência atual do pedal e marcha atual) e fornecer métodos para alterar esse estado, o objeto permanece no controle de como o mundo externo tem permissão para usa-lo. Por exemplo, se a bicicleta tiver apenas 6 marchas, um método para alterar as marchas pode rejeitar qualquer valor < 1  ||  > 6**.

**Agrupar código em objetos de software individuais oferece uma série de benefícios, incluindo**:

1. **Modularidade**: O código-fonte de um objeto pode ser escrito e mantido independente do código-fonte de outros objetos. Uma vez criado, um objeto pode ser facilmente passado dentro do sistema.

2. **Ocultação de informações**: Ao interagir apenas com os métodos de um objeto, os detalhes de sua implementação interna permanecem ocultos do mundo externo.

3. **Reutilização do código**: Se um objeto já existir (talvez escrito por outro desenvolvedor de software), você pode usar esse objeto em seu programa. Isso permite que especialista implementem/testem/depurem objetos complexos e específicos de tarefas, que você pode então confiar para executar em seu próprio código.

4. **Facilidade de plugabilidade e depuração**: Se um objeto em particular se mostrar problemático. você pode simplesmente removê-lo do seu aplicativo e plugar um objeto diferente como seu substituto. Isso é análogo a consertar problemas mecânicos no mundo real. Se um para fuso quebrar, você o substitui, não  máquina inteira. 