# Projeto de Sistema para Campeonato

## 🧑‍💻 Usuários

- **Clientes**: Usuários comuns do sistema, não fazem parte de nenhum time, equipe de gerência ou organização do evento.  
- **Gerentes de Equipe**: Membros das empresas às quais os times pertencem; realizam cadastros de equipes e têm contato com os administradores do evento.  
- **Administradores da Confederação**: Fazem parte da equipe organizadora do evento. Têm acesso total ao sistema para organizar chaveamentos, atualizar informações, gerenciar palpites, etc.

---

## 📋 Documento de Requisitos

### 🔒 Requisitos Não Funcionais (RNF)

- **RNF01** – Login com credenciais válidas.  
- **RNF02** – Usabilidade: sistema intuitivo.  
- **RNF03** – Segurança contra acesso não autorizado.  
- **RNF04** – Respostas rápidas do sistema.  
- **RNF05** – Código padronizado e fácil de manter.  
- **RNF06** – Alta disponibilidade.  
- **RNF07** – Compatível com navegadores web modernos (desktop e mobile).  
- **RNF08** – Backup e recuperação de dados.  
- **RNF09** – Conformidade com normas da instituição.

### ✅ Requisitos Funcionais (RF)

- **RF01** – Visualizar equipes.  
- **RF02** – Visualizar competições.  
- **RF03** – Visualizar resultados e placares.  
- **RF04** – Fazer palpites.  
- **RF05** – Visualizar palpites e resultados.  
- **RF06** – Cadastrar e editar equipes (gerente).  
- **RF07** – Cadastrar e editar membros (gerente).  
- **RF08** – Agendar e gerenciar eventos (admin).  
- **RF09** – Gerenciar palpites (admin).

---

## 📋 Caso de Uso

![image](https://github.com/user-attachments/assets/0136db57-2cda-4b86-a4d5-44444de920b1)

---

# 📘 Narrativa do Sistema “Controle de Campeonato Esportivo (LTA)”

O sistema **Controle de Campeonato Esportivo (LTA)** foi desenvolvido para atender às necessidades dos principais envolvidos em um campeonato esportivo, incluindo **Clientes**, **Gerentes de Equipe** e o **Administrador da Confederação**. A seguir, detalhamos os papéis e os casos de uso de cada ator.

---

## 👤 Cliente

O **Cliente** é o usuário comum do sistema, responsável por acompanhar o campeonato e interagir com funcionalidades relacionadas a jogos e palpites. Ele possui acesso a cinco funcionalidades principais:

- **Visualizar Times**  
  Permite ao cliente conhecer as equipes participantes. Este caso de uso pode ser estendido a partir do cadastro e edição das equipes, realizado pelos gerentes.

- **Visualizar Resultados e Placar**  
  Possibilita ao cliente ver os placares atualizados das partidas. Este caso também pode ser estendido com base nos dados cadastrados pelos outros atores.

- **Visualizar Partidas**  
  Permite acompanhar a programação dos jogos. Esse caso é estendido pelas ações de agendamento de eventos.

- **Fazer Palpite**  
  O cliente pode dar palpites sobre o resultado dos jogos. Este caso de uso inclui o caso **Verificar Palpites**, que possibilita ao cliente acompanhar se seus palpites foram corretos.

- **Verificar Palpites**  
  Este caso estende a funcionalidade **Gerenciar Palpites**, que é realizada pelo administrador.

---

## 👤 Gerente de Equipe

O **Gerente de Equipe** é responsável pelas informações das equipes no sistema. Ele pode:

- **Cadastrar e Editar Equipe**  
  Criar e manter os dados das equipes participantes.

- **Cadastrar e Editar Membros**  
  Adicionar ou modificar os dados dos membros da equipe.

Essas funcionalidades impactam diretamente nos dados que os clientes acessam ao visualizar times e resultados.

---

## 👤 Administrador da Confederação

O **Administrador da Confederação** é o responsável pelas ações organizacionais do campeonato. Ele pode:

- **Agendar e Gerenciar Eventos**  
  Definir as datas e horários dos jogos, o que estende o caso de uso de **Visualizar Partidas** para os clientes.

- **Gerenciar Palpites**  
  Controlar e validar os palpites realizados pelos clientes, o que estende a funcionalidade de **Verificar Palpites**.

---

## 🧩 Relações Entre Casos de Uso

- As setas com `<<extends>>` indicam que determinado caso de uso pode ser complementado com outro. Por exemplo, visualizar times pode ser enriquecido com dados de cadastro feitos pelo gerente.

- A seta com `<<includes>>` entre “Fazer Palpite” e “Verificar Palpites” indica que sempre que um palpite é feito, o sistema deve incluir o recurso de verificação para validar posteriormente os resultados.


---

## Interface

### A interface foi feita por meio do figma

- https://www.figma.com/design/uKipizdqZk7or4YKeKME6m/Untitled?node-id=0-1&p=f&t=Gx92mE684oIMYmJt-0

---

## Métricas Para o Desenvolvimento de Software 

### Conformidade aos prazos:  

- O quão alinhado está o desenvolvimento aos prazos definidos 
- Mede a capacidade de planejamento e organização da equipe 

### Progresso concluído: 

- Quanto do que é esperado de cada entrega e o quanto foi entregue 
- É importante para medir o progresso do sistema e como ele se compara com o planejado 

### Quantidade e impacto de novos bugs: 

- Quantos e o quão impactantes são os eventuais bugs do sistema 
- Serve para dar uma melhor noção de como está a qualidade do desenvolvimento, medindo se a quantidade está dentro do esperado e se a proporção de bugs críticos está baixa 

### Velocidade e qualidade de correção de bugs: 

- O quão rápido os bugs estão sendo corrigidos e o quão efetivas são as soluções aplicadas 
- É importante para medir a capacidade de correção de bugs e pontos em que ela pode ser melhorada 

---

### Burn Down Chart da Atividade

![Grafico Burn](/images/Burn.png)

# Dados Simulados (Linha Real)

## 🗓️ Plano de Sprint (10 Dias) – Projeto Campeonato LTA

Este plano distribui os 18 requisitos (9 funcionais e 9 não funcionais) em um ciclo de desenvolvimento de 10 dias, agrupando tarefas relacionadas para otimizar o fluxo de trabalho.

---

## 📅 Dia 1: Fundação e Segurança  

**Foco:** Estabelecer a base do sistema com autenticação e autorização.

- **RNF01** – Login com credenciais válidas: Implementar a tela e a lógica de login.  
- **RNF03** – Segurança contra acesso não autorizado: Definir e aplicar as permissões para cada tipo de usuário (Cliente, Gerente, Admin).

---

## 📅 Dia 2: Estrutura de Administração  

**Foco:** Construir as funcionalidades centrais para o Administrador organizar o evento.

- **RF08** – Agendar e gerenciar eventos (admin): Permitir que o admin crie e edite as partidas, datas e horários.

---

## 📅 Dia 3: Gerenciamento de Equipes  

**Foco:** Desenvolver as ferramentas para o Gerente de Equipe.

- **RF06** – Cadastrar e editar equipes (gerente): Criar o formulário e a lógica para que gerentes possam adicionar e atualizar suas equipes.  
- **RF07** – Cadastrar e editar membros (gerente): Permitir a gestão dos jogadores/membros dentro de cada equipe.

---

## 📅 Dia 4: Visualização para Clientes  

**Foco:** Criar as principais telas de consulta para o usuário final.

- **RF01** – Visualizar equipes: Listar as equipes participantes.  
- **RF02** – Visualizar competições: Exibir a tabela de jogos e o calendário.

---

## 📅 Dia 5: Interação do Cliente - Palpites  

**Foco:** Implementar a principal funcionalidade interativa do sistema.

- **RF04** – Fazer palpites: Desenvolver a interface para que os clientes possam registrar seus palpites nas partidas agendadas.

---

## 📅 Dia 6: Acompanhamento de Resultados  

**Foco:** Conectar os dados do admin com a visualização do cliente.

- **RF03** – Visualizar resultados e placares: Exibir os placares das partidas finalizadas.  
- **RF05** – Visualizar palpites e resultados: Permitir que o cliente veja seu histórico de palpites e se acertou ou errou.

---

## 📅 Dia 7: Finalização do Ciclo de Palpites  

**Foco:** Dar ao administrador o controle para finalizar e validar os palpites.

- **RF09** – Gerenciar palpites (admin): Implementar a ferramenta para o admin apurar os resultados dos palpites após o fim das partidas.

---

## 📅 Dia 8: Usabilidade e Compatibilidade  

**Foco:** Refinar a experiência do usuário e garantir o funcionamento em diferentes plataformas.

- **RNF02** – Usabilidade: Revisar todo o fluxo do sistema para garantir que seja intuitivo.  
- **RNF07** – Compatível com navegadores web modernos: Testar e corrigir a interface em navegadores como Chrome, Firefox e Safari (desktop e mobile).

---

## 📅 Dia 9: Otimização e Qualidade de Código  

**Foco:** Melhorar o desempenho e a manutenção do código.

- **RNF04** – Respostas rápidas do sistema: Otimizar consultas ao banco de dados e o carregamento das páginas.  
- **RNF05** – Código padronizado e fácil de manter: Refatorar o código e garantir que segue os padrões definidos.

---

## 📅 Dia 10: Disponibilidade e Finalização da Sprint  

**Foco:** Cuidar dos requisitos de infraestrutura, backups e conformidade.

- **RNF06** – Alta disponibilidade: Configurar o ambiente de produção para garantir que o sistema fique online.  
- **RNF08** – Backup e recuperação de dados: Implementar rotinas de backup.  
- **RNF09** – Conformidade com normas da instituição: Realizar a checagem final de todas as regras.

---

# Cronograma de Execução da Sprint

Esta tabela detalha o progresso das tarefas com base no plano de sprint e nos dados do Burndown Chart simulado. Ela mapeia o início planeado de cada requisito com o seu dia de conclusão na simulação.

- **Dia de Início:** O dia em que a tarefa foi agendada para começar, de acordo com o plano de sprint.
- **Dia de Conclusão:** O dia em que a tarefa foi concluída, de acordo com a simulação do burndown (onde a "Linha Real" desce).

| Requisito | Tarefa | Dia de Início | Dia de Conclusão | Status |
| :--- | :--- | :---: | :---: | :--- |
| **RNF01** | Login com credenciais válidas | 1 | 2 | Concluído |
| **RNF03** | Segurança contra acesso não autorizado | 1 | 3 | Concluído |
| **RF08** | Agendar e gerenciar eventos (admin) | 2 | 3 | Concluído |
| **RF06** | Cadastrar e editar equipes (gerente) | 3 | 4 | Concluído |
| **RF07** | Cadastrar e editar membros (gerente) | 3 | 4 | Concluído |
| **RF01** | Visualizar equipes | 4 | 5 | Concluído |
| **RF02** | Visualizar competições | 4 | 5 | Concluído |
| **RF04** | Fazer palpites | 5 | 6 | Concluído |
| **RF03** | Visualizar resultados e placares | 6 | 6 | Concluído |
| **RF05** | Visualizar palpites e resultados | 6 | 7 | Concluído |
| **RF09** | Gerenciar palpites (admin) | 7 | 7 | Concluído |
| **RNF02** | Usabilidade | 8 | 8 | Concluído |
| **RNF07** | Compatível com navegadores web modernos | 8 | 9 | Concluído |
| **RNF04** | Respostas rápidas do sistema | 9 | 9 | Concluído |
| **RNF05** | Código padronizado e fácil de manter | 9 | 10 | Concluído |
| **RNF06** | Alta disponibilidade | 10 | 10 | Concluído |
| **RNF08** | Backup e recuperação de dados | 10 | - | **Pendente** |
| **RNF09** | Conformidade com normas da instituição | 10 | - | **Pendente** |

---

### Análise do Cronograma

- **Início Lento:** As primeiras tarefas (`RNF01`, `RNF03`) levaram um dia a mais para serem concluídas do que o ideal, refletindo o início mais lento visto no gráfico.
- **Recuperação:** A equipe acelerou o ritmo entre os dias 4 e 7, entregando as tarefas dentro do dia esperado.
- **Atraso Final:** As duas últimas tarefas (`RNF08`, `RNF09`) não foram concluídas até o final do Dia 10, o que corresponde aos **2 requisitos restantes** mostrados no Burndown Chart.


## Cálculo de Pontos de Função

| Tipo de Função | Complexidade Funcional | Peso | Quantidade | Total por Complexidade |
| -------------- | ---------------------- | ---- | ---------- | ---------------------- |
| **EE**         | Baixa                  | x 3  | 8          | 24                     |
|                | Média                  | x 4  | 5          | 20                     |
|                | Alta                   | x 6  | 2          | 12                     |
|                |                        |      |            | **Total EE: 49**       |
| **SE**         | Baixa                  | x 4  | 7          | 28                     |
|                | Média                  | x 5  | 5          | 25                     |
|                | Alta                   | x 7  | 1          | 7                      |
|                |                        |      |            | **Total SE: 60**       |
| **CE**         | Baixa                  | x 3  | 0          | 0                      |
|                | Média                  | x 4  | 3          | 12                     |
|                | Alta                   | x 6  | 1          | 6                      |
|                |                        |      |            | **Total CE: 18**       |
| **ALI**        | Baixa                  | x 7  | 1          | 7                      |
|                | Média                  | x 10 | 3          | 30                     |
|                | Alta                   | x 15 | 1          | 15                     |
|                |                        |      |            | **Total ALI: 52**      |
| **AIE**        | Baixa                  | x 5  | 7          | 35                     |
|                | Média                  | x 7  | 1          | 7                      |
|                | Alta                   | x 10 | 1          | 10                     |
|                |                        |      |            | **Total AIE: 52**      |
||||||
|||||**Total Final: 238**|

---

## ✅ Plano de Testes

### 🧪 Casos de Teste Funcionais

| ID       | Tipo | Requisito | Título do Teste                          | Passos / Método                                                                 | Resultado Esperado / Métrica                                                                 |
|----------|------|-----------|------------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------|
| CT-RF01  | RF   | RF01      | Visualizar lista de equipes              | 1. Login como Cliente<br>2. Acessar página "Equipes"                            | Exibir logos e nomes de todas as equipes participantes                                       |
| CT-RF02  | RF   | RF02      | Visualizar competições                   | 1. Acessar "Competições" ou "Calendário"                                        | Listar partidas com times, datas e status (Agendada, Ao Vivo, Finalizada)                   |
| CT-RF03  | RF   | RF03      | Ver resultado de partida finalizada      | 1. Acessar página de Competições<br>2. Selecionar uma partida finalizada        | Mostrar placar final da partida (ex: Time A 2x1 Time B)                                      |
| CT-RF04  | RF   | RF04      | Fazer palpite com sucesso                | 1. Login como Cliente<br>2. Acessar partida agendada<br>3. Fazer palpite        | Mensagem "Palpite realizado com sucesso" e palpite listado no histórico                     |
| CT-RF05  | RF   | RF04      | Impedir palpite após início              | 1. Login como Cliente<br>2. Tentar palpitar em partida ao vivo/finalizada       | Botão desabilitado ou mensagem: "O tempo para palpites encerrou"                            |
| CT-RF06  | RF   | RF05      | Visualizar histórico de palpites         | 1. Login como Cliente<br>2. Acessar "Meus Palpites" no perfil                   | Listar palpites feitos, com status: Pendente, Acertou, Errou                                 |
| CT-RF07  | RF   | RF06      | Cadastrar nova equipe                    | 1. Login como Gerente<br>2. "Minhas Equipes" > "Adicionar Equipe"               | Nova equipe salva e associada ao gerente                                                     |
| CT-RF08  | RF   | RF06      | Editar equipe existente                  | 1. Login como Gerente<br>2. Selecionar e editar equipe                          | Nome atualizado refletido no sistema                                                         |
| CT-RF09  | RF   | RF07      | Adicionar membro à equipe                | 1. Login como Gerente<br>2. Página da equipe > "Adicionar Membro"               | Novo membro adicionado à lista da equipe                                                     |
| CT-RF10  | RF   | RF08      | Agendar evento (partida)                 | 1. Login como Admin<br>2. "Gerenciar Eventos" > Criar partida                   | Partida criada exibida no calendário público                                                 |
| CT-RF11  | RF   | RF09      | Finalizar palpites após partida          | 1. Login como Admin<br>2. Gerenciar partida finalizada e rodar apuração         | Palpites marcados como "Acertou" ou "Errou"                                                  |
| CT-RF12  | RF   | RF09      | Ver relatório de palpites                | 1. Login como Admin<br>2. Selecionar evento > "Relatório de Palpites"           | Exibir número de palpites por equipe                                                         |

---

### 🧪 Casos de Teste Não Funcionais

| ID       | Tipo | Requisito | Título do Teste                              | Passos / Método                                                                 | Resultado Esperado / Métrica                                                                 |
|----------|------|-----------|----------------------------------------------|----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------|
| CT-RNF01 | RNF  | RNF01     | Login com credenciais válidas                | 1. Inserir usuário/senha corretos<br>2. Clicar em "Entrar"                      | Usuário autenticado e redirecionado ao painel                                                |
| CT-RNF02 | RNF  | RNF01     | Login com credenciais inválidas              | 1. Inserir senha errada<br>2. Clicar em "Entrar"                                | Mensagem: "Usuário ou senha inválidos", sem login                                            |
| CT-RNF03 | RNF  | RNF02     | Usabilidade para novo cliente                | Teste com usuário real observando fluxo: cadastro, encontrar partida, palpitar | Tarefas devem ser concluídas em até 3 minutos                                                |
| CT-RNF04 | RNF  | RNF03     | Acesso indevido entre gerentes               | 1. Login como Gerente A<br>2. Tentar acessar edição da Equipe B                | Sistema bloqueia acesso com mensagem de permissão                                            |
| CT-RNF05 | RNF  | RNF04     | Desempenho da página de palpites             | Teste de carga com 1.000 usuários usando JMeter                                | Tempo de resposta inferior a 2 segundos                                                      |
| CT-RNF06 | RNF  | RNF05     | Qualidade do código                          | Análise estática via SonarQube ou ESLint                                       | Sem "code smells" críticos e 95% de conformidade com guia de estilo                         |
| CT-RNF07 | RNF  | RNF06     | Monitoramento de disponibilidade             | Ferramenta como UptimeRobot                                                    | Uptime ≥ 99.9% nos últimos 30 dias                                                           |
| CT-RNF08 | RNF  | RNF07     | Compatibilidade em navegadores               | Teste manual no Chrome (desktop) e Safari (iOS)                                | Fluxo completo deve funcionar sem falhas                                                     |
| CT-RNF09 | RNF  | RNF08     | Verificação da integridade do backup         | Executar script de verificação                                                 | Script deve retornar "Backup OK"                                                             |
| CT-RNF10 | RNF  | RNF08     | Teste de recuperação de backup               | Restaurar backup em ambiente de homologação                                    | Tempo de recuperação (RTO) inferior a 1 hora                                                 |
| CT-RNF11 | RNF  | RNF09     | Verificar exigência de maioridade no palpite | Revisão manual do fluxo                                                        | Confirmação de maioridade deve ser obrigatória e funcional antes do primeiro palpite         |
