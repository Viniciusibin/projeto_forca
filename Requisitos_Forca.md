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




# Requisitos Não Funcionais (RNFs) - Jogo de Forca Online

- **RNF01 - Eficiência de Desempenho (ISO 25010)**  
  - O sistema deve carregar e responder às interações em menos de **2 segundos** para garantir uma experiência fluida ao usuário.  

  - **Critério de Aceitação (CA01):**  
    - O tempo de carregamento das telas deve ser inferior a 2 segundos em 95% dos acessos.  

  - **Teste (T01):**  
    - **Pré-condição:** Acesso a uma conexão de internet padrão.  
    - **Procedimento do teste:** Medir tempo de carregamento em diferentes páginas e ações.  
    - **Resultado esperado:** O sistema carrega dentro do tempo estipulado.  
    - **Pós-condição:** O usuário interage com o sistema sem atrasos perceptíveis.  

- **RNF02 - Conformidade com WCAG 2.1 (ISO 25010)**  
  - O sistema deve ser acessível para usuários com deficiência, seguindo as diretrizes **WCAG 2.1**.  

  - **Critério de Aceitação (CA01):**  
    - Compatibilidade com leitores de tela como **NVDA** e **JAWS**.  

  - **Teste (T01):**  
    - **Pré-condição:** Usuário com leitor de tela ativo.  
    - **Procedimento do teste:** Navegar no sistema e validar acessibilidade dos elementos.  
    - **Resultado esperado:** Todos os elementos são lidos corretamente pelo leitor de tela.  
    - **Pós-condição:** Usuários com deficiência visual conseguem jogar sem dificuldades.  


- **RNF03 - Proteção de Dados (ISO 25010)**  
  - O sistema deve garantir a **proteção de dados dos usuários**, seguindo boas práticas de segurança cibernética.  

  - **Critério de Aceitação (CA01):**  
    - Implementação de autenticação segura e proteção contra ataques comuns, como **SQL Injection** e **Cross-Site Scripting (XSS)**.  

  - **Teste (T01):**  
    - **Pré-condição:** O sistema deve estar implementado com medidas de segurança.  
    - **Procedimento do teste:** Realizar tentativas de acesso indevido e verificar a resistência do sistema.  
    - **Resultado esperado:** Nenhuma vulnerabilidade é explorada com sucesso.  
    - **Pós-condição:** O sistema mantém os dados dos usuários protegidos.  


- **RNF04 - Suporte a um Grande Número de Usuários**  
  - O sistema deve suportar **múltiplos jogadores simultaneamente** sem degradação de desempenho.  

  - **Critério de Aceitação (CA01):**  
    - O servidor deve ser capaz de lidar com **pelo menos 1000 jogadores concorrentes** sem perda de performance.  

  - **Teste (T01):**  
    - **Pré-condição:** Teste de carga com múltiplos usuários conectados simultaneamente.  
    - **Procedimento do teste:** Simular acessos simultâneos e medir o impacto no desempenho.  
    - **Resultado esperado:** O jogo mantém a estabilidade mesmo com alto número de acessos.  
    - **Pós-condição:** O sistema continua operacional sem quedas.  


- **RNF05 - Suporte a Múltiplos Dispositivos e Navegadores**  
  - O jogo deve ser compatível com os **principais navegadores e dispositivos móveis**.  

  - **Critério de Aceitação (CA01):**  
    - O sistema deve ser testado e funcionar corretamente em **Google Chrome, Mozilla Firefox, Microsoft Edge e Safari**.  
    - O jogo deve ser responsivo e adaptar-se corretamente a **smartphones e tablets**.  

  - **Teste (T01):**  
    - **Pré-condição:** Acesso ao sistema a partir de diferentes navegadores e dispositivos.  
    - **Procedimento do teste:** Validar a interface e funcionalidade em cada navegador e dispositivo.  
    - **Resultado esperado:** O jogo mantém sua usabilidade e jogabilidade em todas as plataformas testadas.  
    - **Pós-condição:** Nenhuma funcionalidade essencial é perdida em diferentes dispositivos.  

- **RNF06 - Uptime mínimo garantido**  
  - O sistema deve garantir uma disponibilidade mínima de **99,5%** para evitar interrupções no serviço.  

  - **Critério de Aceitação (CA01):**  
    - O servidor deve ser configurado para manter **alta disponibilidade**, utilizando balanceamento de carga e redundância.  

  - **Teste (T01):**  
    - **Pré-condição:** Sistema hospedado em ambiente de produção com monitoramento ativo.  
    - **Procedimento do teste:** Verificar logs de tempo de atividade ao longo de um mês.  
    - **Resultado esperado:** O tempo de inatividade não deve ultrapassar **0,5%** no período testado.  
    - **Pós-condição:** O sistema continua acessível mesmo em momentos de alta demanda.  

- **RNF07 - Backup Automático de Dados**  
  - O sistema deve realizar **backups automáticos diários** dos dados dos jogadores para evitar perdas.  

  - **Critério de Aceitação (CA01):**  
    - O sistema deve armazenar cópias de segurança dos rankings, estatísticas e configurações dos jogadores.  

  - **Teste (T01):**  
    - **Pré-condição:** O sistema deve estar configurado para realizar backups automáticos.  
    - **Procedimento do teste:** Recuperar dados de backup e verificar sua integridade.  
    - **Resultado esperado:** O sistema restaura os dados corretamente a partir do backup.  
    - **Pós-condição:** Nenhuma perda de informação ocorre após uma eventual falha.  


- **RNF08 - Interface Intuitiva e Atraente**  
  - O jogo deve ter uma interface **clara, responsiva e de fácil navegação** para todos os tipos de usuários.  

  - **Critério de Aceitação (CA01):**  
    - A interface deve seguir princípios de **design UX/UI modernos**, garantindo uma experiência fluida.  

  - **Teste (T01):**  
    - **Pré-condição:** Usuários participando de testes de usabilidade.  
    - **Procedimento do teste:** Realizar testes A/B com diferentes layouts e coletar feedback.  
    - **Resultado esperado:** O layout escolhido apresenta alto nível de satisfação entre os usuários.  
    - **Pós-condição:** O sistema mantém a usabilidade sem necessidade de tutoriais extensivos.  


- **RNF09 - Facilidade de Manutenção**  
  - O código-fonte deve ser estruturado e modular para facilitar **correções, melhorias e novas implementações**.  

  - **Critério de Aceitação (CA01):**  
    - O código deve seguir padrões como **SOLID** e **Clean Code**, além de estar bem documentado.  

  - **Teste (T01):**  
    - **Pré-condição:** Código disponível no repositório com documentação atualizada.  
    - **Procedimento do teste:** Revisão de código e análise estática para verificar boas práticas.  
    - **Resultado esperado:** O código é compreensível e fácil de modificar sem impactos negativos.  
    - **Pós-condição:** O sistema permanece flexível para futuras atualizações.  


- **RNF10 - Baixo Consumo de Recursos**  
  - O jogo deve ser otimizado para **minimizar o consumo de CPU, memória e banda de rede**.  

  - **Critério de Aceitação (CA01):**  
    - O sistema deve ser capaz de rodar em dispositivos **com configurações modestas**, sem causar travamentos.  

  - **Teste (T01):**  
    - **Pré-condição:** Jogo executado em dispositivos de diferentes níveis de hardware.  
    - **Procedimento do teste:** Medir consumo de memória, CPU e largura de banda.  
    - **Resultado esperado:** O consumo de recursos permanece dentro dos limites definidos.  
    - **Pós-condição:** O jogo roda suavemente em dispositivos menos potentes.  


- **RNF11 - Latência Máxima Aceitável**  
  - O sistema deve garantir que todas as ações do jogo tenham um **tempo de resposta inferior a 300ms** para evitar atrasos perceptíveis pelos jogadores.  

  - **Critério de Aceitação (CA01):**  
    - O tempo entre a entrada do jogador (ex: escolha de uma letra) e a atualização da interface não pode ultrapassar **300ms** em 95% dos casos.  

  - **Teste (T01):**  
    - **Pré-condição:** Conexão de internet padrão (mínimo 10 Mbps) e servidor operando normalmente.  
    - **Procedimento do teste:** Simular ações dos jogadores e medir o tempo de resposta do sistema.  
    - **Resultado esperado:** O tempo médio de resposta para cada ação é menor que **300ms**.  
    - **Pós-condição:** O jogo mantém uma experiência fluida e responsiva para os usuários.  




