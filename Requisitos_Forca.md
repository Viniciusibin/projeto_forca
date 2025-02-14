# Levantamento de Requisitos - Jogo de Forca Online

## Requisitos Funcionais (RFs):

- **RF01: O sistema deve permitir que os usuários criem e participem de partidas online de forca.**
  - **CA01:** O sistema deve disponibilizar um mecanismo para criar e ingressar em partidas públicas e privadas.
  - **T01:** Criar uma partida e validar se outros usuários podem ingressar.
    - **Pré-condição:** O usuário deve estar logado.
    - **Procedimento do teste:** Criar uma partida e verificar se outro usuário pode ingressar.
    - **Resultado esperado:** Outro usuário consegue ingressar na partida corretamente.
    - **Pós-condição:** O sistema inicia a partida com os jogadores conectados.

- **RF02: O sistema deve permitir partidas multiplayer em tempo real.**
  - **CA01:** O jogo deve permitir que dois ou mais jogadores participem simultaneamente.
  - **T01:** Criar uma partida com múltiplos jogadores e validar a interação em tempo real.
    - **Pré-condição:** Múltiplos usuários conectados.
    - **Procedimento do teste:** Criar uma partida, adicionar jogadores e verificar o funcionamento da rodada.
    - **Resultado esperado:** Os jogadores conseguem jogar alternadamente sem atrasos.
    - **Pós-condição:** O sistema mantém a sincronia entre os jogadores.

- **RF03: O sistema deve oferecer um chat para comunicação entre os jogadores.**
  - **CA01:** O chat deve permitir envio e recebimento de mensagens durante a partida.
  - **T01:** Enviar e receber mensagens no chat da partida.
    - **Pré-condição:** Usuários conectados em uma partida.
    - **Procedimento do teste:** Enviar mensagens entre jogadores e verificar a recepção.
    - **Resultado esperado:** As mensagens são entregues corretamente em tempo real.
    - **Pós-condição:** O chat permanece ativo durante toda a partida.

- **RF04: O sistema deve armazenar estatísticas dos jogadores.**
  - **CA01:** O sistema deve registrar número de vitórias, derrotas e palavras acertadas.
  - **T01:** Jogar múltiplas partidas e verificar se os dados estão sendo armazenados corretamente.
    - **Pré-condição:** Usuário logado e participando de partidas.
    - **Procedimento do teste:** Jogar partidas e acessar as estatísticas após o jogo.
    - **Resultado esperado:** Os dados do jogador são atualizados corretamente.
    - **Pós-condição:** As estatísticas são mantidas corretamente no banco de dados.

- **RF05: O jogo deve ter um sistema de pontos para gerar um ranking de jogadores.**
  - **CA01:** O sistema deve calcular pontos com base no desempenho dos jogadores.
  - **T01:** Jogar múltiplas partidas e verificar a atualização do ranking.
    - **Pré-condição:** Usuários cadastrados e participando de partidas.
    - **Procedimento do teste:** Conferir a atualização do ranking após cada partida.
    - **Resultado esperado:** O ranking reflete corretamente o desempenho dos jogadores.
    - **Pós-condição:** O ranking é atualizado dinamicamente.

- **RF06: O jogo deve estar disponível em pelo menos três línguas: Inglês, Português e Espanhol.**
  - **CA01:** O usuário deve poder selecionar a língua da interface.
  - **T01:** Alternar entre os idiomas e verificar a tradução correta.
    - **Pré-condição:** Opção de troca de idioma implementada.
    - **Procedimento do teste:** Alterar idioma e verificar a tradução dos textos na interface.
    - **Resultado esperado:** Os textos são exibidos corretamente no idioma selecionado.
    - **Pós-condição:** O usuário consegue jogar no idioma desejado.

- **RF07: O jogador deve poder escolher o tema das palavras do jogo.**
  - **CA01:** O sistema deve oferecer diferentes temas, como animais, esportes e tecnologia.
  - **T01:** Escolher um tema e verificar se as palavras geradas correspondem ao tema selecionado.
    - **Pré-condição:** Sistema configurado com múltiplos temas.
    - **Procedimento do teste:** Selecionar um tema e iniciar uma partida.
    - **Resultado esperado:** Todas as palavras geradas pertencem ao tema escolhido.
    - **Pós-condição:** O jogador tem controle sobre a temática do jogo.

- **RF08: O sistema deve permitir que jogadores criem salas privadas com senha.**  
  - **CA01:** O usuário deve poder criar uma sala e definir uma senha para acesso.  
  - **T01:** Criar uma sala privada e validar se apenas jogadores com a senha conseguem acessá-la.  
    - **Pré-condição:** O usuário deve estar logado e criar uma sala privada.  
    - **Procedimento do teste:** Criar uma sala privada, compartilhar a senha com outro jogador e tentar ingressar.  
    - **Resultado esperado:** Apenas jogadores com a senha conseguem entrar.  
    - **Pós-condição:** A sala permanece protegida contra acessos indevidos.  

- **RF09: O jogo deve ter um sistema de dicas para ajudar os jogadores.**  
  - **CA01:** O sistema deve permitir o uso de uma dica por rodada.  
  - **T01:** Jogar uma partida e solicitar uma dica.  
    - **Pré-condição:** O jogador deve estar participando da partida.  
    - **Procedimento do teste:** Solicitar uma dica e verificar se a informação fornecida é relevante para a palavra oculta.  
    - **Resultado esperado:** O sistema exibe uma dica útil sem revelar diretamente a palavra.  
    - **Pós-condição:** O jogador pode continuar tentando adivinhar a palavra com mais informações.  

- **RF10: O sistema deve permitir que os jogadores personalizem seus avatares.**  
  - **CA01:** O usuário pode selecionar um avatar entre opções pré-definidas ou carregar uma imagem.  
  - **T01:** Selecionar um avatar e verificar se ele aparece corretamente durante o jogo.  
    - **Pré-condição:** O usuário deve estar logado.  
    - **Procedimento do teste:** Escolher um avatar e iniciar uma partida.  
    - **Resultado esperado:** O avatar escolhido é exibido corretamente durante o jogo.  
    - **Pós-condição:** O avatar permanece salvo para futuras partidas.  

- **RF11: O jogo deve permitir torneios com múltiplas rodadas.**  
  - **CA01:** O sistema deve permitir a criação de torneios com fases eliminatórias.  
  - **T01:** Criar um torneio e verificar a progressão das rodadas.  
    - **Pré-condição:** Múltiplos jogadores cadastrados.  
    - **Procedimento do teste:** Criar um torneio, adicionar jogadores e acompanhar as eliminações por rodada.  
    - **Resultado esperado:** O torneio avança corretamente até definir um vencedor.  
    - **Pós-condição:** Os jogadores eliminados não continuam nas rodadas seguintes.  

- **RF12: O sistema deve permitir diferentes modos de jogo.**  
  - **CA01:** O usuário pode escolher entre modos como Clássico, Temporizado e Desafio.  
  - **T01:** Selecionar um modo de jogo e validar suas regras específicas.  
    - **Pré-condição:** O usuário deve estar na tela de configuração da partida.  
    - **Procedimento do teste:** Escolher um modo de jogo e verificar se as regras são aplicadas corretamente.  
    - **Resultado esperado:** O jogo segue as regras do modo escolhido.  
    - **Pós-condição:** O jogador pode alternar entre diferentes modos para mais variedade.  
