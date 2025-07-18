# Análise de Requisitos - Aplicativo "PodSpot"



 
Este projeto foi criado com objetivo de praticar o **levantamento de requisitos** funcionais e não funcionais do aplicativo móvel "PodSpot", com base na primeira versão do protótipo de telas fornecidas para o projeto. O objetivo é estabelecer uma compreensão clara das funcionalidades esperadas do sistema, servindo como base para o desenvolvimento, testes e validação do produto.

## Visão Geral
O PodSpot é um aplicativo mobile para descoberta, organização e reprodução de podcasts. O objetivo é centralizar o acesso aos principais podcasts, permitindo ao usuário navegar por categorias, visualizar detalhes dos programas, ouvir episódios e gerenciar suas preferências.

### Escopo do Projeto
O escopo inicial do projeto **PodSpot**, conforme as telas analisadas, abrange as seguintes áreas principais, que representam as funcionalidades essenciais para a primeira versão do aplicativo:

- Experiência de onboarding para novos usuários.

- Navegação e descoberta de podcasts e categorias.

- Visualização de detalhes de podcasts.

- Listagem e reprodução de episódios.

- Funcionalidades básicas de gerenciamento de reprodução.

- Filtro de ordenação.



### Protótipo
**Versão: 1.0**
- protótipo do figma: [PodSpot](https://www.figma.com/design/ECIzSfAWHcPJSi3HxkKdUr/PodcastAppChallenge?m=auto&t=WBSxPDFw8EJ0oCFy-1)



### Requisitos Funcionais 
Os requisitos estão organizados por tela do aplicativo, as **User Stories**, as **Regras de Negócio** e os **Critérios de Aceite**.
Para os Critérios de Aceite, utilizamos a linguagem Gherkin (BDD).
<br>

### Tela 01: Tela Inicial (Onboarding)
<br>

![Referência  Protótipo](/img/tela_de_onbording.png)


### Descrição da Tela:
É a primeira tela que o usuário vê ao abrir o aplicativo, com o logotipo do PodSpot, uma breve descrição e um botão para iniciar.

### User Stories: 
Como um novo usuário, eu quero ver uma tela de boas-vindas com uma breve descrição do aplicativo para entender sua proposta.

### Regras de Negócio:
**RN01.01:** A tela inicial deve conter o nome do aplicativo "PodSpot".

**RN01.02:** Deve haver uma frase descritiva: "Listen to all of your favorite podcasts in one spot.".

**RN01.03:** Deve haver um botão de ação com o texto "Get Started".
<br>
<br>

### Critérios de Aceite (Gherkin - BDD):
<br>

### Cenário: Visualização da tela inicial

**Dado** que o aplicativo PodSpot é aberto pela primeira vez 

**Quando** a tela inicial é carregada

**Então** o título "PodSpot" deve ser exibido na tela

**E** a descrição "Listen to all of your favorite podcasts in one spot." deve ser exibida

**E** o botão "Get Started" deve ser exibido e estar clicável.
<br>
<br>

### Cenário: Navegação a partir do botão "Get Started"

**Dado** que estou na tela inicial do aplicativo PodSpot.

**Quando** eu toco no botão "Get Started".

**Então** serei direcionado para a tela principal (home) do aplicativo.
<br>
<br>

### Tela 02: Tela Principal (Home): 

![Referência  Protótipo](/img/tela_home%20.png)

### Descrição da Tela:
Exibe um conteúdo diversificado como "Top 10 Podcasts", "Categories" e "Recommended", além de uma barra de navegação inferior.

### User Stories:

**US02.01:** "Como um usuário, eu quero poder explorar diferentes conteúdos (Top 10 Podcasts, Categorias, Recomendações) na tela principal para descobrir novos podcasts."

**US02.02:** "Como um usuário, eu quero acessar rapidamente as principais seções do aplicativo (Home, Microfone, Pesquisa, Perfil) através da barra de navegação para otimizar minha experiência."


### Regras de Negócio:
**RN02.01:** A tela principal deve exibir a seção "Top 10 Podcasts" com miniaturas e títulos para cada podcast.

**RN02.02:** A seção "Categories" deve exibir categorias visíveis e um botão "See All".

**RN02.03:** A seção "Recommended" deve exibir miniaturas de podcasts e um botão "See All".

**RN02.04:** Deve haver um ícone de perfil no canto superior direito.

**RN02.05:** A barra de navegação inferior deve conter os ícones "Home", "Microfone" e "Pesquisa".
<br>
<br>

### Critérios de Aceite (Gherkin - BDD):
<br>

### Cenário: Visualização dos elementos da tela Home

**Dado** que estou na tela principal do aplicativo PodSpot.

**Quando** a tela é carregada.

**Então** a seção "Top 10 Podcasts" deve ser visível com pelo menos 3 podcasts exibidos.

**E** a seção "Categories" deve ser visível com pelo menos 4 categorias e o botão "See All".

**E** a seção "Recommended" deve ser visível com pelo menos 3 podcasts e o botão "See All".

**E** o ícone de perfil deve ser exibido no canto superior direito.

**E** a barra de navegação inferior com os ícones "Home", "Microfone" e "Pesquisa" deve ser exibida e funcional.
<br>
<br>

### Cenário: Navegação para a tela de detalhes do Podcast

**Dado** que estou na tela principal do aplicativo PodSpot

**Quando** eu toco em um dos podcasts da seção "Top 10 Podcasts" (ex: "The Official PodSpot Podcast").

**Então** serei direcionado para a tela de detalhes do podcast selecionado.
<br>
<br>

### Tela 03: Tela de Detalhes do Podcast

![Referência  Protótipo](/img/tela_detalhes-do_podacst.png)


### Descrição da Tela:
Exibe informações detalhadas sobre um podcast específico, incluindo sua capa, título, descrição e uma lista de episódios recentes.

### User Stories:
**US03.01:** "Como um usuário, eu quero visualizar informações detalhadas de um podcast (título, descrição, imagem de capa) para entender sobre o conteúdo."

**US03.02:** "Como um usuário, eu quero ver uma lista dos episódios recentes de um podcast para escolher qual ouvir."

**US03.03:** "Como um usuário, eu quero ter opções de navegação (voltar) e interação (favoritar podcast) na tela de detalhes para gerenciar minha experiência."


### Regras de Negócio:

**RN03.01:** A tela deve exibir a imagem de capa e o título do podcast ("The Official PodSpot Podcast").

**RN03.02:** A descrição do podcast deve ser exibida, e se for longa, deve haver a opção "see more".

**RN03.03**: A classificação "TOP 10 PODCAST" deve ser visível, se aplicável.

**RN03.04:** Deve haver uma seção com o título "Recent Episodes".

**RN03.05:** O primeiro episódio na seção "Recent Episodes" deve exibir título e duração ("Episode 102", "37 min").

**RN03.06:** Deve haver um ícone de "voltar" (seta para a esquerda) no canto superior esquerdo.

**RN03.07:** Deve haver um ícone de coração no canto superior direito para favoritar o podcast.
<br>
<br>

### Critérios de Aceite (Gherkin - BDD):
<br>

### Cenário: Visualização dos detalhes do podcast

**Dado** que eu naveguei para a tela de detalhes de um podcast.

**Quando** a tela é carregada.

**Então** a imagem de capa e o título do podcast devem ser exibidos.

**E** a descrição do podcast deve ser visível, com a opção "see more" se o texto ultrapassar 3 linhas.

**E** a classificação "TOP 10 PODCAST" deve ser exibida.

**E** a seção "Recent Episodes" deve ser visível com o título do episódio e sua duração.

**E** o ícone de "voltar" deve ser exibido e estar clicável.

**E** o ícone de coração para favoritar deve ser exibido e estar clicável.
<br>
<br>

### Cenário: Navegação para a lista completa de episódios

**Dado** que estou na tela de detalhes do podcast.

**Quando** eu toco na área do primeiro episódio recente ("Episode 102").

**Então** serei direcionado para a tela de lista de episódios.
<br>
<br>

### Cenário: Voltar para a tela anterior

**Dado** que estou na tela de detalhes do podcast.

**Quando** eu toco no ícone de "voltar" (seta para a esquerda).

**Então** serei direcionado de volta para a tela principal (home).
<br>
<br>

### Tela 04: Tela de Lista de Episódios

![Referência  Protótipo](/img/tela_epsodios_recentes.png)


### Descrição da Tela:
Exibe uma lista de todos os episódios de um podcast, com informações detalhadas e opções de reprodução.

### User Stories:
**US04.01:** "Como um usuário, eu quero visualizar uma lista completa dos episódios de um podcast, incluindo título, descrição, duração e data de lançamento, para ter todas as informações relevantes."

**US04.02:** "Como um usuário, eu quero iniciar a reprodução de um episódio diretamente da lista para começar a ouvir rapidamente."

**US04.03:** "Como um usuário, eu quero ver quais episódios já escutei na lista para acompanhar meu progresso."

**US04.04:** "Como um usuário, eu quero ter opções de navegação (voltar) e filtragem/ordenação na lista de episódios para organizar e encontrar o que desejo."

### Regras de Negócio:
**RN04.01:** A tela deve exibir o título "Episodes".

**RN04.02:** Cada item de episódio na lista deve exibir: título, descrição breve, data de lançamento e duração.

**RN04.03:** Cada episódio deve ter um ícone de "play" visível e clicável para iniciar a reprodução.

**RN04.04:** Episódios que já foram escutados devem exibir um ícone de checkmark.

**RN04.05:** Deve haver um ícone de "voltar" (seta para a esquerda) no canto superior esquerdo.

**RN04.06:** Deve haver um ícone de filtro/ordenar no canto superior direito.
<br>
<br>

### Critérios de Aceite (Gherkin - BDD):
<br>

### Cenário: Visualização da lista de episódios

**Dado** que eu naveguei para a tela de lista de episódios.

**Quando** a tela é carregada.

**Então** o título "Episodes" deve ser exibido.

**E** uma lista de episódios deve ser exibida, cada um com título, descrição, data e duração.

**E** para cada episódio, o ícone de "play" deve ser visível.

**E** episódios como "Episode 102" e "Episode 100" devem exibir o ícone de checkmark.

**E** o ícone de "voltar" deve ser exibido e estar clicável.

**E** o ícone de filtro/ordenar deve ser exibido e estar clicável.
<br>
<br>

### Cenário: Reprodução de um episódio a partir da lista

**Dado** que estou na tela de lista de episódios

**Quando** eu toco no ícone de "play" de um episódio (ex: "Episode 102").

**Então** serei direcionado para a tela de reprodução do episódio.
<br>
<br>

### Cenário: Voltar para a tela anterior

**Dado** que estou na tela de lista de episódios.

**Quando** eu toco no ícone de "voltar" (seta para a esquerda).

**Então** serei direcionado de volta para a tela de detalhes do podcast.
<br>
<br>

### Tela 05: Tela de Reprodução do Episódio

![Referência  Protótipo](/img/tela_de_reproducao.png)

### Descrição da Tela:
Exibe a interface para a reprodução de um episódio de podcast, incluindo controles de áudio e barra de progresso.

### User Stories:
**US05.01:** "Como um usuário, eu quero visualizar o título e o nome do podcast na tela de reprodução para saber o que estou ouvindo."

**US05.02:** "Como um usuário, eu quero controlar a reprodução de áudio (play, pause, pular para frente/trás) e ver o progresso para ter controle total sobre a experiência de audição."

**US05.03:** "Como um usuário, eu quero ter opções de navegação (voltar) e acesso a 'mais opções' na tela de reprodução para gerenciar o episódio."

### Regras de Negócio:
**RN05.01:** A tela deve exibir o título do episódio ("Episode 102").

**RN05.02:** O nome do podcast ("The Official PodSpot Podcast") deve ser exibido abaixo do título do episódio.

**RN05.03:** Deve haver uma barra de progresso do áudio indicando o tempo decorrido (ex: "0:00") e o tempo total (ex: "37:01").

**RN05.04:** A tela deve conter os botões de controle de reprodução: "voltar 10 segundos", "play/pause" e "avançar 10 segundos".

**RN05.05:** Deve haver um ícone de "voltar" (seta para a esquerda) no canto superior esquerdo.

**RN05.06:** Deve haver um ícone de três pontos no canto superior direito para "mais opções".
<br>
<br>

### Critérios de Aceite (Gherkin - BDD):
<br>

### Cenário: Visualização da tela de reprodução

**Dado** que eu iniciei a reprodução de um episódio.

**Quando** a tela de reprodução é carregada.

*Então* o título do episódio e o nome do podcast devem ser exibidos.

**E** a barra de progresso do áudio deve ser visível, mostrando o tempo decorrido e o tempo total do episódio.

**E** os botões "voltar", "play/pause" e "avançar" devem ser exibidos e estar clicáveis.

**E** o ícone de "voltar" deve ser exibido e estar clicável.

**E** o ícone de três pontos (mais opções) deve ser exibido e estar clicável.
<br>
<br>

### Cenário: Controle de reprodução - Pausar

**Dado** que um episódio está sendo reproduzido na tela de reprodução.

**Quando** eu clico no botão de "play/pause".

**Então** a reprodução deve pausar.

**E** o ícone do botão deve mudar para "play".
<br>
<br>

### Cenário: Controle de reprodução - Iniciar

**Dado** que um episódio está pausado na tela de reprodução.

**Quando** eu toco no botão de "play/pause".

**Então** a reprodução deve reiniciar.

**E** o ícone do botão deve mudar para "pause".
<br>
<br>

### Cenário: Voltar para a tela anterior

**Dado** que estou na tela de reprodução do episódio.

**Quando** eu toco no ícone de "voltar" (seta para a esquerda).

**Então** serei direcionado de volta para a tela de lista de episódios.
<br>
<br>

### Cenário: Mais opções de comando

**Dado** que estou na tela de reprodução do episódio.

**Quando** eu clico no ícone de "Três pontos" (mais opções).

**Então** exibirá um drawer vertical com mais opções de comando para acessar.
<br>
<br>

### Requisitos Não Funcionais 

Descrevem como o sistema deve se comportar, abrangendo aspectos como desempenho, usabilidade, segurança e confiabilidade. Apesar de as telas fornecidas focarem nas funcionalidades, podemos inferir os seguintes requisitos não funcionais essenciais para o sucesso do aplicativo "PodSpot".

### A prioridade
Indica a importância do RNF para o sucesso do projeto e do produto. É uma medida do "nível de risco" associado ao RNF.

**Alta:** Essencial para o funcionamento básico, segurança, conformidade legal ou que causa grande impacto negativo se não atendido. Geralmente, falhas nesse RNF impediriam o lançamento do produto.

**Média:** Importante para a experiência do usuário, desempenho otimizado ou eficiência operacional, mas não impede completamente o lançamento em uma versão inicial.

**Baixa:** Desejável, mas não crítico para a funcionalidade principal ou para a experiência imediata. Pode ser implementado em versões futuras.

### A Origem 
Explica de onde o requisito foi derivado ou por que ele existe.

**Inferido do Protótipo:** Significa que o RNF foi deduzido a partir da análise das telas e do fluxo do aplicativo, mesmo que não estivesse explicitamente escrito.

**Boa Prática de Mercado:** Baseado em padrões da indústria, expectativas comuns de usuários para aplicativos similares ou recomendações de usabilidade/desempenho.

**Requisito de Negócio/Stakeholder:** Derivado de uma necessidade explícita do negócio ou de um stakeholder (mesmo que, neste exercício, você esteja simulando o levantamento).

**Norma/Legislação:** Requisitos ditados por leis, regulamentações ou normas técnicas (como a ISO/IEC 25010 que você já mencionou para classificação).
<br>
<br>

### Desempenho (Performance Efficiency)

**NFR01:** O aplicativo deve carregar a tela inicial em no máximo 3 segundos em redes 4G/Wi-Fi.

>**Prioridade: Alta** (Carga inicial impacta diretamente a primeira impressão e retenção do usuário, crucial para o sucesso).

>**Origem: Boa Prática de Mercado** (Expectativa de usuários por aplicativos rápidos), **Inferido do Protótipo** (Aplicativos modernos devem ser rápidos).

**NFR02:** "A transição entre as telas (Home, Detalhes do Podcast, Lista de Episódios, Reprodução) deve ser fluida e ocorrer em no máximo 1 segundo."

>**Prioridade: Alta** (Fluidez na navegação é essencial para a usabilidade e experiência do usuário).

>**Origem: Boa Prática de Mercado** (Padrão de experiência de usuário para apps mobile).

**NFR03:** "A reprodução de um episódio deve iniciar em no máximo 2 segundos após o clique no botão 'Play', considerando uma conexão de internet estável."

>**Prioridade: Alta** (Impacta diretamente a função principal do aplicativo: ouvir podcasts. Atrasos aqui causariam frustração imediata).

>**Origem: Inferido do Protótipo** (Função central da reprodução), **Boa Prática de Mercado.**

**NFR04:** "A barra de progresso da reprodução deve ser atualizada em tempo real, sem atrasos perceptíveis."

>**Prioridade: Média** (Um leve atraso não impede o uso, mas afeta a usabilidade).

>**Origem: Inferido do Protótipo** (Representação visual da progressão), **Boa Prática de Mercado.**
<br>
<br>

### Usabilidade (Usability)

**NFR05:** "A interface do usuário deve ser intuitiva e de fácil navegação, permitindo que um usuário encontre e reproduza um podcast em no máximo 3 cliques a partir da tela principal."

>**Prioridade: Alta** (Diretamente ligada à satisfação do usuário e ao objetivo de "facilitar a descoberta").

>**Origem: Inferido do Protótipo** (Layout visa facilidade), **Requisito de Negócio** (Facilidade de uso é um diferencial competitivo), **Boa Prática de Mercado.**

**NFR06:** "Os ícones e textos devem ser claros e legíveis em diferentes tamanhos de tela e orientações (retrato/paisagem)."

>**Prioridade: Alta** (Essencial para acessibilidade e uso em diversos dispositivos).

>**Origem: Boa Prática de Mercado** (Design responsivo), Norma (Padrões de acessibilidade inferidos).

**NFR07:** "O feedback visual para ações do usuário (ex: clique em botões, carregamento de conteúdo) deve ser imediato e claro."

>**Prioridade: Média** (Impacta a percepção de responsividade e evita que o usuário clique múltiplas vezes).

>**Origem: Boa Prática de Mercado** (Design de UX/UI).

**NFR08:** "O aplicativo deve ser responsivo a toques, sem atrasos na resposta da interface."

>**Prioridade: Alta** (A falta de resposta a toques torna o aplicativo inutilizável).

>**Origem: Boa Prática de Mercado** (Expectativa básica de aplicativos móveis).
<br>
<br>

### Confiabilidade (Reliability)

**NFR09:** "O aplicativo deve ser estável e não apresentar crashes inesperados durante o uso contínuo (ex: após 4 horas de reprodução ininterrupta)."

>**Prioridade: Altíssima** (Crashes destroem a experiência do usuário e a reputação do aplicativo).

>**Origem: Requisito de Negócio** (Qualidade fundamental do produto), Boa Prática de Mercado.

**NFR10:** "A reprodução de áudio deve ser contínua e sem interrupções inesperadas, a menos que a conexão com a internet seja perdida."

>**Prioridade: Alta** (Diretamente relacionada à função principal e à satisfação do usuário).

>**Origem: Requisito de Negócio, Boa Prática de Mercado.**

**NFR11:** "O progresso do episódio deve ser salvo automaticamente, permitindo que o usuário retome a reprodução de onde parou."

>**Prioridade: Média** (Importante para a conveniência do usuário, mas não impede a funcionalidade principal).

>**Origem: Boa Prática de Mercado** (Recurso comum em players de áudio/vídeo).
<br>
<br>

### Segurança (Security)

**NFR12:** "Caso haja funcionalidades de login/cadastro (inferido pelo ícone de perfil), os dados do usuário devem ser protegidos com criptografia adequada (ex: HTTPS para comunicação, criptografia para dados armazenados)."

>**Prioridade: Altíssima** (Questões de privacidade e conformidade legal).

>**Origem: Inferido do Protótipo** (Presença de perfil), Norma (GDPR, LGPD ou outras regulamentações de dados), Boa Prática de Mercado.

**NFR13:** "O aplicativo deve proteger contra acessos não autorizados a informações ou funcionalidades restritas do usuário."

>**Prioridade: Altíssima** (Prevenção de fraudes e acesso indevido a dados).

>**Origem: Requisito de Negócio, Boa Prática de Mercado.**
<br>
<br>

### Compatibilidade (Compatibility)

**NFR14:** O aplicativo deve ser compatível com as versões mais recentes dos sistemas operacionais móveis (iOS e Android) e suas duas versões anteriores.

**NFR15:** O aplicativo deve funcionar corretamente em diferentes tamanhos e resoluções de tela de dispositivos móveis.
<br>
<br>
### Manutenibilidade (Maintainability)

**NFR16:** O código-fonte do aplicativo deve seguir padrões de codificação e ser bem documentado para facilitar futuras manutenções e evoluções. (Este é um requisito mais interno, mas crucial para a longevidade do produto).

>**Prioridade: Média** (Impacta o custo e a velocidade de desenvolvimento a longo prazo).

>**Origem: Boa Prática de Mercado** (Engenharia de Software), Requisito de Negócio (Redução de custos futuros).
