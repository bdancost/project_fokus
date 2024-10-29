# Fokus

### Descrição

O projeto **Fokus** é um site desenvolvido para otimizar a produtividade dos usuários, oferecendo uma ferramenta de temporizador que alterna entre períodos de foco, descanso curto e descanso longo. O objetivo é ajudar os usuários a manterem-se concentrados em suas tarefas, ao mesmo tempo em que realizam pausas para evitar fadiga. Este projeto é fictício e não possui fins comerciais.

### Funcionalidades

- **Temporizador Dinâmico**: O site permite que o usuário escolha entre três contextos de temporização:
  - **Foco**: um período de 25 minutos para concentração profunda.
  - **Descanso Curto**: uma pausa rápida de 5 minutos.
  - **Descanso Longo**: uma pausa estendida de 15 minutos.
- **Alternância de Contexto**: Botões interativos que mudam o contexto da aplicação, alterando o visual do site e o tempo do temporizador conforme a opção escolhida.
- **Controle de Música**: Possibilidade de ativar ou desativar música ambiente durante o período de foco, com controle de som simples por meio de um botão toggle.
- **Início/Pausa do Temporizador**: Um botão central para iniciar e pausar o temporizador, que ajusta automaticamente o ícone e o texto conforme o estado atual.
- **Feedback Sonoro**: Efeitos sonoros são reproduzidos ao iniciar ou pausar o temporizador, além de um som de alarme ao término do período de foco.

### Ferramentas e Tecnologias

- **HTML5**: Estrutura básica do site, utilizando semântica moderna para melhor organização e acessibilidade do conteúdo.
- **CSS3**: Estilização avançada com variáveis de cores, gradientes e design responsivo para adaptar a interface a diferentes dispositivos (desktop, tablet e mobile).
- **JavaScript**: Lógica de interação e comportamento do site, garantindo uma experiência dinâmica para o usuário.

### Funcionalidades Detalhadas em JavaScript

- **Controle do Contexto de Temporizador**:
  - Manipulação da propriedade `data-contexto` do elemento `html` para alterar o tema de fundo de acordo com o contexto selecionado (foco, descanso curto ou longo).
  - Uso de `querySelector` e `addEventListener` para detectar cliques nos botões de contexto e atualizar a interface conforme necessário.
  - Ajuste visual dos botões para destacar a seleção ativa.
- **Controle do Temporizador**:

  - Utilização de `setInterval` para gerenciar a contagem regressiva do temporizador.
  - Funções de controle para iniciar, pausar e zerar o tempo, com a possibilidade de alternar o texto e ícone do botão de controle entre "Começar" e "Pausar".
  - Cálculo do tempo restante e exibição formatada no elemento do temporizador na tela.

- **Reprodução de Áudio**:

  - Implementação de `Audio` para reproduzir sons específicos:
    - Música de fundo durante o período de foco.
    - Sons de início e pausa do temporizador.
    - Alerta sonoro ao término do tempo.
  - Controle do som de fundo com um checkbox que ativa ou desativa a música ambiente.

- **Feedback Visual e Responsividade**:
  - Manipulação dinâmica de classes para alterar a aparência de elementos, garantindo que a interface responda a diferentes ações do usuário.
  - Ajuste da interface com CSS flexbox e media queries para garantir que o site seja acessível e visualmente atraente em dispositivos de diversos tamanhos.

### Estrutura do Projeto

- **index.html**: Estrutura HTML do site, organizando os elementos principais como o temporizador, botões de controle e conteúdo visual.
- **styles.css**: Estilos personalizados para garantir um design moderno e responsivo, utilizando gradientes e variáveis de CSS.
- **script.js**: Lógica de interação e temporização, controle de música e atualização dinâmica da interface.

### Como Executar o Projeto

1. Clone este repositório:
   ```bash
   git clone https://github.com/usuario/fokus.git
   ```
2. Navegue até a pasta do projeto:
   ```bash
   cd fokus
   ```
3. Abra o arquivo `index.html` em um navegador de sua escolha.
