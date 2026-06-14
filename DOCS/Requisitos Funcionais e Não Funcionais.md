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
