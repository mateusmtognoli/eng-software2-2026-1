# 💊 ReMed - Sistema de Gerenciamento de Medicamentos

  ![Engenharia de Software](https://img.shields.io/badge/Engenharia%20de%20Software-II-green)
  ![Status](https://img.shields.io/badge/status-em%20desenvolvimento-orange)

## 📌 Descrição

⭢ O ReMed é um aplicativo desenvolvido para auxiliar usuários — especialmente idosos e seus cuidadores — no controle do uso correto de medicamentos.

⭢ O sistema permite cadastrar remédios, configurar alarmes, enviar notificações e registrar o histórico de ingestão, garantindo mais segurança e organização no tratamento.

#####

## 🎥 Apresentação do Projeto

Para uma melhor compreensão do funcionamento do sistema, foi desenvolvida um vídeo de apresentação demonstrando suas principais funcionalidades, objetivos e estrutura.

Nela, são abordados:

⭢ Dores resolvidas

⭢ Diagrama de Casos de Uso

⭢ Diagrama de Classes

⭢ Apresentação do protótipo

---

[Clique aqui para ver o vídeo de apresentação](https://youtu.be/zbpmw8rTQWk)

####

## 🎯 Objetivos

⭢ Garantir o uso correto dos medicamentos  
⭢ Reduzir esquecimentos e falhas no tratamento  
⭢ Facilitar o acompanhamento por cuidadores  
⭢ Melhorar a organização da rotina de medicação  
⭢ Aumentar a segurança e autonomia do paciente  
⭢ Oferecer uma interface simples e acessível  

#####

## 👥 Atores / Personas

- Usuário (Responsável)

⭢ Realiza o cadastro e autenticação no sistema

⭢ Gerencia seus dependentes e suas informações pessoais

⭢ Cadastra, edita e remove medicamentos dos dependentes

⭢ Acompanha o histórico e as estatísticas de adesão ao tratamento

⭢ Monitora o estoque dos medicamentos e recebe informações sobre sua disponibilidade

---

- Dependente

⭢ Representa a pessoa que faz uso dos medicamentos cadastrados

⭢ Possui informações médicas e pessoais para auxiliar no acompanhamento do tratamento

⭢ Tem sua rotina de medicação monitorada pelo sistema

⭢ Possui registros de adesão utilizados para acompanhamento da administração dos medicamentos

⭢ Está vinculado a um usuário responsável pelo gerenciamento de seus dados

---

- Administrador

⭢ Gerencia o funcionamento geral do sistema  
⭢ Monitora desempenho e disponibilidade  
⭢ Analisa dados e indicadores de uso  
⭢ Garante segurança e integridade dos dados  
⭢ Realiza manutenção e atualizações do sistema  

---

[Clique aqui para ver as Personas](DOCS/PERSONAS)

####

## 👥 Público-Alvo

⭢ Idosos

⭢ Pacientes em tratamento contínuo

⭢ Cuidadores e familiares

#####

## ⚠️ Principais Dores

⭢ Esquecimento de horários de medicamentos  
⭢ Falta de controle sobre doses tomadas  
⭢ Dificuldade de acompanhamento por cuidadores  
⭢ Erros na administração (dosagem/intervalo)  
⭢ Falta de organização no tratamento  

#####

## ⚙️ Requisitos Funcionais

| ID   | Requisito | Categoria |
|------|-----------|-----------|
| RF01 | O sistema deve permitir o cadastro de usuário com nome, e-mail, senha e preenchimento de dados complementares no primeiro acesso (tipo sanguíneo, CPF, data de nascimento, altura, peso, telefone). | Autenticação e Conta |
| RF02 | O sistema deve permitir login com e-mail e senha, com opção "lembrar-me" e recuperação de senha por e-mail. | Autenticação e Conta |
| RF03 | O sistema deve permitir a exclusão de conta com apagamento de todos os dados associados, incluindo índices de emparelhamento. | Autenticação e Conta |
| RF04 | O sistema deve permitir o cadastro de medicamento com nome, dosagem, instruções, horário, dias da semana e categoria. | Gestão de Medicamentos |
| RF05 | O sistema deve permitir a confirmação de dose com status Tomada ou Pulada, e marcar automaticamente como Atrasada quando o horário agendado passar sem confirmação. | Gestão de Medicamentos |
| RF06 | O sistema deve realizar o reset automático diário dos status das doses (Tomada/Pulada → Pendente) à meia-noite, acumulando o histórico de adesão do dia encerrado. | Gestão de Medicamentos |
| RF07 | O sistema deve permitir a remoção de medicamento da agenda. | Gestão de Medicamentos |
| RF08 | O sistema deve permitir o cadastro de itens no estoque com nome, tipo (comprimido, cápsula, líquido, ampola) e quantidade inicial. | Gestão de Estoque |
| RF09 | O sistema deve reduzir automaticamente o estoque ao confirmar uma dose como Tomada, com base na quantidade definida na dosagem. | Gestão de Estoque |
| RF10 | O sistema deve permitir a reposição manual de estoque com quantidade personalizada e atualizar o total de referência para cálculo de alertas. | Gestão de Estoque |
| RF11 | O sistema deve gerar alertas automáticos de estoque Crítico (≤ 10% do total registrado) e Alerta (< 30%), com indicação visual por cores. | Gestão de Estoque |
| RF12 | O sistema deve exibir o histórico de doses da semana corrente com filtros por status (Tomadas, Atrasadas, Puladas, Pendentes). | Histórico e Relatórios |
| RF13 | O sistema deve calcular e exibir o percentual de adesão por dependente, combinando histórico acumulado de dias anteriores com as ações do dia atual. | Histórico e Relatórios |
| RF14 | O sistema deve permitir a geração e download de relatório em PDF com doses e estoque, disponível por dependente individualmente ou consolidado para todos. | Histórico e Relatórios |
| RF15 | O sistema deve permitir o cadastro de dependente com dados pessoais e informações médicas (tipo sanguíneo, alergias, condições de saúde, plano de saúde), gerando automaticamente um código de emparelhamento. | Dependentes e Emparelhamento |
| RF16 | O sistema deve permitir o emparelhamento de dispositivo secundário via código, atribuindo o papel Emparelhado com acesso restrito. | Dependentes e Emparelhamento |
| RF17 | O sistema deve permitir a alternância entre dependentes pelo responsável, bem como o desemparelhamento ou remoção de dependente. | Dependentes e Emparelhamento |
| RF18 | O sistema deve exibir um centro de notificações com alertas de doses pendentes, atrasadas, confirmadas, puladas e estoque crítico, com ação rápida de confirmação diretamente na tela. | Notificações |
| RF19 | O sistema deve permitir que o usuário configure suas preferências de notificação (medicamentos, estoque, resumo diário, relatório mensal, adesão). | Notificações |
| RF20 | O sistema deve oferecer gerenciamento de segurança da conta: alteração de senha, ativação de autenticação em duas etapas (2FA) por e-mail e visualização de sessões ativas com opção de encerrar outras sessões. | Segurança |


#####


## 🛠️ Requisitos Não Funcionais

| ID    | Requisito | Categoria |
|-------|-----------|-----------|
| RNF01 | O sistema deve ser um aplicativo mobile, disponível para Android e iOS. | Plataforma |
| RNF02 | O sistema deve verificar doses atrasadas e realizar o reset diário sem bloqueio da interface. | Desempenho |
| RNF03 | O sistema deve apresentar animações de transição entre telas e componentes sem impacto perceptível na navegação. | Desempenho |
| RNF04 | O sistema deve isolar os dados por conta, escopando todas as chaves de armazenamento pelo identificador do usuário. | Segurança |
| RNF05 | O sistema deve proteger rotas privadas com guarda de autenticação, redirecionando automaticamente para o login quando não autenticado. | Segurança |
| RNF06 | O sistema deve controlar o acesso por responsável ou emparelhado, impedindo que o usuário emparelhado cadastre, altere ou reponha medicamentos e estoque. | Segurança |
| RNF07 | O sistema deve apresentar interface totalmente intuitiva, com formatação de datas, valores e máscaras de campos (CPF, telefone, altura, peso) | Usabilidade |
| RNF08 | O sistema deve fornecer feedback visual imediato em todas as ações, incluindo estados de carregamento, mensagens de sucesso/erro e animações de confirmação. | Usabilidade |
| RNF09 | O sistema deve indicar o status do estoque com código de cores (verde = normal, amarelo = alerta, vermelho = crítico). | Usabilidade |
| RNF10 | O sistema deve funcionar offline no estado atual de protótipo, sem dependência de servidor externo. | Disponibilidade |
| RNF11 | O sistema deve pré-carregar dados de demonstração automaticamente na primeira sessão para facilitar a avaliação do produto. | Disponibilidade |

#####

## 📝 Casos de Uso

Os casos de uso representam as interações entre os diferentes tipos de usuários e o sistema, descrevendo suas funcionalidades principais.

O sistema foi projetado considerando dois tipos de atores principais:

⭢ Dependente (Conta Emparelhada)

⭢ Responsável

⭢ Administrador

---

👤 Dependente (Conta Emparelhada)

O paciente dependente possui acesso simplificado, focado no acompanhamento das medicações e recebimento de informações enviadas pelo responsável.

⭢ UCD01: Visualizar notificações

⭢ UCD02: Visualizar dashboard (próximas doses)

⭢ UCD03: Visualizar histórico de doses

⭢ UCD04: Emparelhar celular ao responsável

⭢ UCD05: Sair da conta (logout)

---

👨‍👩‍👧 Responsável

O responsável possui acesso completo às funcionalidades de gerenciamento de medicamentos, estoque, notificações, segurança e administração dos dependentes.

- Autenticação e Conta

⭢ UC01: Cadastrar-se

⭢ UC02: Completar dados adicionais

⭢ UC03: Realizar login

⭢ UC04: Recuperar senha

⭢ UC05: Editar perfil

⭢ UC06: Excluir conta

⭢ UC07: Sair da conta (logout)

- Segurança

⭢ UC08: Alterar senha

⭢ UC09: Configurar autenticação de dois fatores

⭢ UC10: Gerenciar sessões ativas

- Gerenciamento de Medicamentos

⭢ UC11: Visualizar dashboard (próximas doses)

⭢ UC12: Adicionar medicamento

⭢ UC13: Registrar dose tomada

⭢ UC14: Visualizar histórico de doses

- Controle de Estoque

⭢ UC15: Adicionar item ao estoque

⭢ UC16: Visualizar estoque

⭢ UC17: Repor estoque

- Notificações

⭢ UC18: Visualizar notificações

⭢ UC19: Configurar preferências de notificação

- Gerenciamento de Acessos

⭢ UC20: Adicionar dependente

⭢ UC21: Gerar código de emparelhamento

⭢ UC22: Gerenciar cuidadores e solicitações

---

🛠️ Administrador

O administrador possui acesso às funcionalidades de supervisão e gerenciamento do sistema, sendo responsável por acompanhar o funcionamento da plataforma e visualizar informações gerais sobre os usuários e recursos cadastrados.

⭢ UCADM01: Gerenciar sistema

⭢ UCADM02: Monitorar desempenho do sistema

⭢ UCADM03: Visualizar dashboard administrativo

⭢ UCADM04: Visualizar responsáveis cadastrados

⭢ UCADM05: Visualizar dependentes cadastrados

⭢ UCADM06: Visualizar medicamentos cadastrados

⭢ UCADM07: Visualizar relatórios e estatísticas

⭢ UCADM08: Realizar manutenção do sistema

⭢ UCADM09: Gerenciar backups

---

- Diagramas de Casos de Uso
  
[Clique aqui para ver os diagramas de casos de uso](https://github.com/mateusmtognoli/eng-software2-2026-1/tree/main/DOCS/CASOS%20DE%20USO)

####

## 🧩 Diagrama de Classes

O diagrama de classes apresenta a estrutura do sistema ReMed, descrevendo suas principais entidades, atributos, enumerações e relacionamentos, modelados conforme os princípios da orientação a objetos e da UML.

- Entidades:

O sistema é composto pelas seguintes classes principais:

⭢ Responsável

⭢ Dependente

⭢ Medicamento

⭢ ItemEstoque

⭢ EstatisticaAdesao

⭢ Notificacao

⭢ Administrador

Além das enumerações:

⭢ StatusMedicamento

⭢ StatusEstoque

⭢ TipoNotificacao

⭢ DiasSemana

---

- Relacionamentos:

⭢ Um Responsável pode possuir zero ou vários Dependentes, sendo responsável pelo gerenciamento de seus dados e tratamentos.

⭢ Cada Dependente está associado a exatamente um Responsável.

⭢ Um Dependente pode possuir zero ou vários Medicamentos cadastrados para acompanhamento do tratamento.

⭢ Cada Medicamento pertence a exatamente um Dependente.

⭢ Um Dependente pode possuir zero ou vários registros de EstatisticaAdesao, utilizados para monitorar a adesão ao tratamento ao longo do tempo.

⭢ Cada registro de EstatisticaAdesao pertence a exatamente um Dependente.

⭢ Um Medicamento pode gerar zero ou várias Notificações, utilizadas para lembretes, alertas de atraso ou avisos relacionados ao tratamento.

⭢ Um Responsável pode receber zero ou várias Notificações.

⭢ Cada Notificação está associada a um único Responsável.

⭢ Cada Notificação utiliza a enumeração TipoNotificacao, que define sua categoria (Lembrete, Atraso ou Estoque).

⭢ A enumeração DiasSemana é utilizada para representar os dias em que notificações e medicamentos podem ser programados.

⭢ Um Medicamento pode estar associado a zero ou um ItemEstoque, permitindo o controle da quantidade disponível.

⭢ Cada ItemEstoque está vinculado a um único Medicamento.

⭢ A classe Medicamento utiliza a enumeração StatusMedicamento para representar o estado atual da administração da dose (Pendente, Tomado, Atrasado ou Pulado).

⭢ A classe ItemEstoque utiliza a enumeração StatusEstoque para indicar a situação do estoque (Normal, Alerta ou Crítico).

⭢ A classe Administrador possui dependências com as entidades Responsável, Dependente, Medicamento e Relatórios e Estatísticas, representando sua capacidade de gerenciamento e supervisão do sistema.

---

- Observações Técnicas:

⭢ O modelo utiliza composição para representar relações de forte dependência entre as entidades, como entre Responsável e Dependente, Dependente e Medicamento, e Dependente e EstatisticaAdesao.

⭢ O diagrama emprega associações com multiplicidades, evidenciando a cardinalidade dos relacionamentos entre as classes.

⭢ As enumerações StatusMedicamento, StatusEstoque, TipoNotificacao e DiasSemana foram modeladas como tipos específicos para garantir a consistência dos dados e das regras de negócio.

⭢ Os identificadores das entidades são representados por atributos do tipo String, podendo ser implementados utilizando UUID para assegurar unicidade.

⭢ A entidade Notificacao permite o gerenciamento de alertas e lembretes enviados aos usuários, armazenando informações como título, mensagem, data, canal de envio e status de leitura.

⭢ A entidade ItemEstoque possibilita o monitoramento da disponibilidade de medicamentos, incluindo quantidade atual, quantidade registrada e status do estoque.

⭢ A entidade EstatisticaAdesao fornece métricas de acompanhamento do tratamento, registrando doses tomadas, total de doses previstas e percentual de adesão.

⭢ O modelo contempla funcionalidades de gerenciamento de usuários, dependentes, medicamentos, notificações, controle de estoque, acompanhamento da adesão ao tratamento e administração do sistema, servindo como base para a implementação do ReMed.

---

[Clique aqui para acessar o diagrama de classes](DOCS/Diagrama-de-Classes-ReMed.png)

#####

## 💻 Prototipação

A prototipação do sistema foi realizada com o objetivo de visualizar a interface do usuário e validar a experiência antes da implementação.

Foram desenvolvidos protótipos de alta fidelidade, representando as principais telas do sistema, como:

   ⭢ Tela de login e cadastro

   ⭢ Dashboard do usuário

   ⭢ Cadastro de medicamentos

   ⭢ Gerenciamento de Estoque

   ⭢ Configuração de horários e alarmes

   ⭢ Histórico de ingestão


Os protótipos permitiram identificar melhorias na usabilidade, organização das informações e fluxo de navegação, garantindo uma experiência mais intuitiva para o usuário final.

---

- Ferramentas utilizadas:

  ⭢ Google Stitch

  ⭢ Google AI Studio

---

- Preview do Protótipo

![Dashboard do Responsável](https://github.com/mateusmtognoli/eng-software2-2026-1/blob/main/DOCS/IMAGENS%20PROTOTIPO/Tela-Inicial-Responsavel-ReMed.jpeg)
![Dashboard do Dependente](https://github.com/mateusmtognoli/eng-software2-2026-1/blob/main/DOCS/IMAGENS%20PROTOTIPO/Tela-Inicial-Dependente-ReMed.jpeg)

---

- Acesso ao Protótipo

Caso queira visualizar o protótipo completo, acesse:

[Protótipo](https://ais-pre-xvhpc3wsfkklewlz4lgn44-157702196272.us-west2.run.app/login)

####

## 🛠️ Tecnologias Previstas

- Frontend: React Native
- Backend: TypeScript
- Banco de Dados: Supabase/Firebase

####

## 👨‍💻 Membros

⭢ **João Pedro Soares**

⭢ **Julia Espiñeira**

⭢ **Mateus Marcondes Tognoli**

⭢ **Mariah Paula Rocha**

⭢ **Reynaldo José Ramos**

#####

## 📄 Licença

Este projeto é acadêmico e pode ser utilizado para fins educacionais.
