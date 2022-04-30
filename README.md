# Os 12 Fatores de um Aplicativo

## Introdução
Na era moderna, o software é comumente entregue como um serviço: chamado de aplicativos da Web ou software como serviço . O aplicativo de doze fatores é uma metodologia para criar aplicativos de software como serviço que:

Use formatos declarativos para automação de configuração, para minimizar tempo e custo para novos desenvolvedores ingressando no projeto;
Ter um contrato limpo com o sistema operacional subjacente, oferecendo máxima portabilidade entre ambientes de execução;
São adequados para implantação em modernas plataformas em nuvem , dispensando a necessidade de administração de servidores e sistemas;
Minimize a divergência entre desenvolvimento e produção, permitindo implantação contínua para máxima agilidade;
E pode escalar sem alterações significativas nas ferramentas, arquitetura ou práticas de desenvolvimento.
A metodologia de doze fatores pode ser aplicada a aplicativos escritos em qualquer linguagem de programação e que usam qualquer combinação de serviços de apoio (banco de dados, fila, cache de memória, etc).

## Fundo
Os colaboradores deste documento estiveram diretamente envolvidos no desenvolvimento e implantação de centenas de aplicativos e testemunharam indiretamente o desenvolvimento, operação e dimensionamento de centenas de milhares de aplicativos por meio de nosso trabalho na plataforma Heroku .

Este documento sintetiza toda a nossa experiência e observações em uma ampla variedade de aplicativos de software como serviço disponíveis. É uma triangulação de práticas ideais para o desenvolvimento de aplicativos, prestando atenção especial à dinâmica do crescimento orgânico de um aplicativo ao longo do tempo, à dinâmica de colaboração entre os desenvolvedores que trabalham na base de código do aplicativo e evitando o custo da erosão do software .

Nossa motivação é aumentar a conscientização sobre alguns problemas sistêmicos que vimos no desenvolvimento de aplicativos modernos, fornecer um vocabulário compartilhado para discutir esses problemas e oferecer um conjunto de soluções conceituais amplas para esses problemas com a terminologia que os acompanha. O formato é inspirado nos livros de Martin Fowler Patterns of Enterprise Application Architecture and Refactoring .

## Quem deve ler este documento?
Qualquer desenvolvedor que cria aplicativos que são executados como um serviço. Engenheiros de operações que implantam ou gerenciam esses aplicativos.

## Os doze fatores

I. Base de código
Uma base de código rastreada no controle de revisão, muitas implantações

II. Dependências
Declare e isole explicitamente dependências

III. Configuração
Armazenar a configuração no ambiente

IV. Serviços de apoio
Trate os serviços de apoio como recursos anexados

V. Construir, liberar, executar
Estágios de compilação e execução estritamente separados

VI. Processos
Execute o aplicativo como um ou mais processos sem estado

VII. Vinculação de porta
Exportar serviços via ligação de porta

VIII. Simultaneidade
Escale horizontalmente por meio do modelo de processo

IX. Descartabilidade
Maximize a robustez com inicialização rápida e desligamento normal

X. Paridade de desenvolvimento/produção
Mantenha o desenvolvimento, a preparação e a produção o mais semelhante possível

XI. Histórico
Tratar logs como streams de eventos

XII. Processos administrativos
Execute tarefas de administração/gerenciamento como processos únicos
