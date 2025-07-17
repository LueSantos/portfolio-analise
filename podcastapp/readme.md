# Análise de Requisitos - Aplicativo "PodSpot"



 
Este projeto foi criado com objetivo de praticar o **levantamento de requisitos** funcionais e não funcionais do aplicativo móvel "Podspot", com base na primeira versão do protótipo de telas fornecidas para o projeto. O objetivo é estabelecer uma compreensão clara das funcionalidades esperadas do sistema, servindo como base para o desenvolvimento, testes e validação do produto.

## Visão Geral
O PodSpot é um aplicativo mobile para descoberta, organização e reprodução de podcasts. O objetivo é centralizar o acesso aos principais podcasts, permitindo ao usuário navegar por categorias, visualizar detalhes dos programas, ouvir episódios e gerenciar suas preferências.

### Escopo do Projeto
O escopo inicial do projeto **PodSpot**, conforme as telas analisadas, abrange as seguintes áreas principais:

- Experiência de onboarding para novos usuários.

- Navegação e descoberta de podcasts e categorias.

- Visualização de detalhes de podcasts.

- Listagem e reprodução de episódios.

- Funcionalidades básicas de gerenciamento de reprodução.

- Filtro de ordenação.



### Protótipo
**Versão: 1.0**
 - protótipo do figma: [PodSpot](https://www.figma.com/design/ECIzSfAWHcPJSi3HxkKdUr/PodcastAppChallenge?m=auto&t=WBSxPDFw8EJ0oCFy-1)



### Requisitos Detalhados 
Os requisitos estão organizados por tela do aplicativo, as **User Stories**, as **Regras de Negócio** e os **Critérios de Aceite**.
Para os Critérios de Aceite, utilizamos a linguagem Gherkin (BDD).
<br>

#### Tela 01: Tela Inicial (Onboarding)
<br>

![Referência  Protótipo](/img/tela_de_onbording.png)


##### Descrição da Tela:
 É a primeira tela que o usuário vê ao abrir o aplicativo, com o logotipo do Podspot, uma breve descrição e um botão para iniciar.

##### User Stories: 
Como um novo usuário, eu quero ver uma tela de boas-vindas com uma breve descrição do aplicativo para entender sua proposta.

##### Regras de Negócio:
**RN01.01:** A tela inicial deve conter o nome do aplicativo "Podspot".
**RN01.02:** Deve haver uma frase descritiva: "Listen to all of your favorite podcasts in one spot.".
**RN01.03:** Deve haver um botão de ação com o texto "Get Started".
<br>

##### Critérios de Aceite (Gherkin - BDD):
<br>

**Cenário: Visualização da tela inicial**
**Dado** que o aplicativo Podspot é aberto pela primeira vez
**Quando** a tela inicial é carregada
**Então** o título "Podspot" deve ser exibido na tela
**E** a descrição "Listen to all of your favorite podcasts in one spot." deve ser exibida
**E** o botão "Get Started" deve ser exibido e estar clicável.
<br>

**Cenário: Navegação a partir do botão "Get Started"**
**Dado** que estou na tela inicial do aplicativo Podspot.
**Quando** eu toco no botão "Get Started".
**Então** serei direcionado para a tela principal (home) do aplicativo.
<br>

#### Tela 02: Tela Principal (Home)1: 

![Referência  Protótipo](/img/tela_home%20.png)

**Descrição da Tela:** Exibe um conteúdo diversificado como "Top 10 Podcasts", "Categories" e "Recommended", além de uma barra de navegação inferior.

##### User Stories:

Como um usuário, **eu quero** poder explorar e navegar facilmente pelo aplicativo, visualizando diferentes conteúdos como "Top 10 Podcasts", "Categorias" e "Recomendações".  Acessar o meu perfil e utilizar uma barra de navegação para as seções principais (Home, Microfone, Pesquisa) para que eu possa acessar de forma rápida simples.


##### Regras de Negócio:
**RN02.01:** A tela principal deve exibir a seção "Top 10 Podcasts" com miniaturas e títulos para cada podcast.
**RN02.02:** A seção "Categories" deve exibir categorias visíveis e um botão "See All".
**RN02.03:** A seção "Recommended" deve exibir miniaturas de podcasts e um botão "See All".
**RN02.04:** Deve haver um ícone de perfil no canto superior direito.
**RN02.05:** A barra de navegação inferior deve conter os ícones "Home", "Microfone" e "Pesquisa".
<br>

##### Critérios de Aceite (Gherkin - BDD):
<br>

**Cenário: Visualização dos elementos da tela Home**
**Dado** que estou na tela principal do aplicativo Podspot.
**Quando** a tela é carregada.
**Então** a seção "Top 10 Podcasts" deve ser visível com pelo menos 3 podcasts exibidos.
**E** a seção "Categories" deve ser visível com pelo menos 4 categorias e o botão "See All".
**E** a seção "Recommended" deve ser visível com pelo menos 3 podcasts e o botão "See All".
**E** o ícone de perfil deve ser exibido no canto superior direito.
**E** a barra de navegação inferior com os ícones "Home", "Microfone" e "Pesquisa" deve ser exibida e funcional.
<br>

**Cenário: Navegação para a tela de detalhes do Podcast**
**Dado** que estou na tela principal do aplicativo Podspot.
**Quando** eu toco em um dos podcasts da seção "Top 10 Podcasts" (ex: "The Official Podspot Podcast").
**Então** serei direcionado para a tela de detalhes do podcast selecionado.


#### Tela 03: Tela de Detalhes do Podcast

![Referência  Protótipo](/img/tela_detalhes-do_podacst.png)


**Descrição da Tela:** Exibe informações detalhadas sobre um podcast específico, incluindo sua capa, título, descrição e uma lista de episódios recentes.

##### User Stories:
Como um usuário, eu quero poder visualizar os detalhes de um podcast (título, descrição, imagem de capa), uma lista de episódios recentes e também ter as opções de navegação (voltar) e interação (favoritar) para que eu possa navegar de forma simples e salvar os episódios favoritos.


##### Regras de Negócio:

**RN03.01:** A tela deve exibir a imagem de capa e o título do podcast ("The Official Podspot Podcast").
**RN03.02:** A descrição do podcast deve ser exibida, e se for longa, deve haver a opção "see more".
**RN03.03**: A classificação "TOP 10 PODCAST" deve ser visível, se aplicável.
**RN03.04:** Deve haver uma seção com o título "Recent Episodes".
**RN03.05:** O primeiro episódio na seção "Recent Episodes" deve exibir título e duração ("Episode 102", "37 min").
**RN03.06:** Deve haver um ícone de "voltar" (seta para a esquerda) no canto superior esquerdo.
**RN03.07:** Deve haver um ícone de coração no canto superior direito para favoritar o podcast.
<br>

##### Critérios de Aceite (Gherkin - BDD):
<br>

**Cenário: Visualização dos detalhes do podcast**
**Dado** que eu naveguei para a tela de detalhes de um podcast.
**Quando** a tela é carregada.
**Então** a imagem de capa e o título do podcast devem ser exibidos.
**E** a descrição do podcast deve ser visível, com a opção "see more" se o texto ultrapassar 3 linhas.
**E** a classificação "TOP 10 PODCAST" deve ser exibida.
**E** a seção "Recent Episodes" deve ser visível com o título do episódio e sua duração.
**E** o ícone de "voltar" deve ser exibido e estar clicável.
**E** o ícone de coração para favoritar deve ser exibido e estar clicável.
<br>

**Cenário: Navegação para a lista completa de episódios**
**Dado** que estou na tela de detalhes do podcast.
**Quando** eu toco na área do primeiro episódio recente ("Episode 102").
**Então** serei direcionado para a tela de lista de episódios.
<br>

**Cenário: Voltar para a tela anterior**
**Dado** que estou na tela de detalhes do podcast.
**Quando** eu toco no ícone de "voltar" (seta para a esquerda).
**Então** serei direcionado de volta para a tela principal (home).
<br>

#### Tela 04: Tela de Lista de Episódios

![Referência  Protótipo](/img/tela_epsodios_recentes.png)


**Descrição da Tela:** Exibe uma lista de todos os episódios de um podcast, com informações detalhadas e opções de reprodução.

##### User Stories:
Como um usuário, eu quero poder visualizar uma lista completa de episódios de um podcast, com detalhes como título, descrição, duração e data de lançamento, ter a opção de reproduzir, identificar episódios já escutados e ter opções de navegação (voltar) e filtragem/ordenação para que eu possa navegar de forma simples.

##### Regras de Negócio:
**RN04.01:** A tela deve exibir o título "Episodes".
**RN04.02:** Cada item de episódio na lista deve exibir: título, descrição breve, data de lançamento e duração.
**RN04.03:** Cada episódio deve ter um ícone de "play" visível e clicável para iniciar a reprodução.
**RN04.04:** Episódios que já foram escutados devem exibir um ícone de checkmark.
**RN04.05:** Deve haver um ícone de "voltar" (seta para a esquerda) no canto superior esquerdo.
**RN04.06:** Deve haver um ícone de filtro/ordenar no canto superior direito.


##### Critérios de Aceite (Gherkin - BDD):

**Cenário: Visualização da lista de episódios**
**Dado** que eu naveguei para a tela de lista de episódios.
**Quando** a tela é carregada.
**Então** o título "Episodes" deve ser exibido.
**E** uma lista de episódios deve ser exibida, cada um com título, descrição, data e duração.
**E** para cada episódio, o ícone de "play" deve ser visível.
**E** episódios como "Episode 102" e "Episode 100" devem exibir o ícone de checkmark.
**E** o ícone de "voltar" deve ser exibido e estar clicável.
**E** o ícone de filtro/ordenar deve ser exibido e estar clicável.
<br>

**Cenário: Reprodução de um episódio a partir da lista**
**Dado** que estou na tela de lista de episódios.
**Quando** eu toco no ícone de "play" de um episódio (ex: "Episode 102").
**Então** serei direcionado para a tela de reprodução do episódio.
<br>

**Cenário: Voltar para a tela anterior**
**Dado** que estou na tela de lista de episódios.
**Quando** eu toco no ícone de "voltar" (seta para a esquerda).
**Então** serei direcionado de volta para a tela de detalhes do podcast.
<br>

#### Tela 05: Tela de Reprodução do Episódio

![Referência  Protótipo](/img/tela_de_reproducao.png)

**Descrição da Tela:** Exibe a interface para a reprodução de um episódio de podcast, incluindo controles de áudio e barra de progresso.

##### User Stories:
Como um usuário, eu quero poder visualizar o título do episódio e o podcast ao qual ele pertence, controlar a reprodução do áudio (play, pause, pular para frente/trás), ver o progresso da reprodução, ter a opção de retornar à tela anterior e ter mais opções para que eu possa acessar outros comandos.

##### Regras de Negócio:
**RN05.01:** A tela deve exibir o título do episódio ("Episode 102").
**RN05.02:** O nome do podcast ("The Official Podspot Podcast") deve ser exibido abaixo do título do episódio.
**RN05.03:** Deve haver uma barra de progresso do áudio indicando o tempo decorrido (ex: "0:00") e o tempo total (ex: "37:01").
**RN05.04:** A tela deve conter os botões de controle de reprodução: "voltar 10 segundos", "play/pause" e "avançar 10 segundos".
**RN05.05:** Deve haver um ícone de "voltar" (seta para a esquerda) no canto superior esquerdo.
**RN05.06:** Deve haver um ícone de três pontos no canto superior direito para "mais opções".
<br>

##### Critérios de Aceite (Gherkin - BDD):

**Cenário: Visualização da tela de reprodução**
**Dado** que eu iniciei a reprodução de um episódio.
**Quando** a tela de reprodução é carregada.
*Então* o título do episódio e o nome do podcast devem ser exibidos.
**E** a barra de progresso do áudio deve ser visível, mostrando o tempo decorrido e o tempo total do episódio.
**E** os botões "voltar", "play/pause" e "avançar" devem ser exibidos e estar clicáveis.
**E** o ícone de "voltar" deve ser exibido e estar clicável.
**E** o ícone de três pontos (mais opções) deve ser exibido e estar clicável.
<br>

**Cenário: Controle de reprodução - Pausar**
**Dado** que um episódio está sendo reproduzido na tela de reprodução.
**Quando** eu clico no botão de "play/pause".
**Então** a reprodução deve pausar.
**E** o ícone do botão deve mudar para "play".
<br>

**Cenário: Controle de reprodução - Iniciar**
**Dado** que um episódio está pausado na tela de reprodução.
**Quando** eu toco no botão de "play/pause".
**Então** a reprodução deve reiniciar.
**E** o ícone do botão deve mudar para "pause".
<br>

**Cenário: Voltar para a tela anterior**
**Dado** que estou na tela de reprodução do episódio.
**Quando** eu toco no ícone de "voltar" (seta para a esquerda).
**Então** serei direcionado de volta para a tela de lista de episódios.
<br>

**Cenário: Mais opções de comando**
**Dado** que estou na tela de reprodução do episódio.
**Quando** eu clico no ícone de "Três pontos" (mais opções)
**Então** exibirá um drawer vertical com mais opções de comando para acessar.