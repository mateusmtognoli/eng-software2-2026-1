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

- Paciente

⭢ Utiliza o sistema para controlar seus medicamentos  
⭢ Recebe alertas nos horários corretos  
⭢ Confirma a ingestão dos remédios  
⭢ Precisa de uma interface simples e acessível  
⭢ Pode visualizar seu histórico de uso  

---

- Cuidador / Responsável

⭢ Acompanha o uso de medicamentos do paciente  
⭢ Recebe notificações caso o medicamento não seja tomado  
⭢ Auxilia na organização da rotina de medicação  
⭢ Monitora o histórico de ingestão  
⭢ Pode gerenciar medicamentos do paciente  

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

####

## ⚙️ Requisitos Funcionais

| ID   | Requisito | Categoria |
|------|----------|----------|
| RF01 | O sistema deve permitir cadastrar medicamentos com nome, dosagem e horário. | Cadastro |
| RF02 | O sistema deve permitir configurar alarmes para horários específicos de cada medicamento. | Alerta/Notificação |
| RF03 | O sistema deve enviar notificações no momento do horário do medicamento. | Notificação |
| RF04 | O sistema deve permitir confirmar a ingestão do medicamento. | Registro |
| RF05 | O sistema deve registrar o histórico de medicamentos tomados e não tomados. | Histórico |
| RF06 | O sistema deve permitir editar e excluir medicamentos cadastrados. | Cadastro |
| RF07 | O sistema deve emitir alertas recorrentes caso o usuário não confirme o uso do medicamento. | Alerta/Notificação |
| RF08 | O sistema deve permitir cadastrar múltiplos usuários (ex: responsável e dependente). | Usuário |
| RF09 | O sistema deve enviar notificações para cuidadores quando o medicamento não for tomado. | Notificação |
| RF10 | O sistema deve permitir configurar lembretes com som, vibração ou ambos. | Configuração |
| RF11 | O sistema deve exibir uma lista diária dos medicamentos a serem tomados. | Visualização |
| RF12 | O sistema deve permitir o cadastro de instruções adicionais (ex: "tomar com comida"). | Cadastro |
| RF13 | O sistema deve funcionar offline para alarmes já configurados. | Sistema |
| RF14 | O sistema deve permitir repetição de medicamentos (diário, semanal, etc.). | Configuração |
| RF15 | O sistema deve permitir configurar intervalo entre doses (ex: a cada 8 horas). | Configuração |
| RF16 | O sistema deve permitir o controle do estoque de medicamentos pelo usuário. | Usuário |

#####


## 🛠️ Requisitos Não Funcionais

| ID    | Requisito | Categoria |
|-------|----------|----------|
| RNF01 | O sistema deve ter interface simples e intuitiva, adequada para idosos. | Usabilidade |
| RNF02 | O sistema deve apresentar tempo de resposta inferior a 2 segundos para ações comuns. | Desempenho |
| RNF03 | O sistema deve garantir disponibilidade de 99% do tempo. | Disponibilidade |
| RNF04 | O sistema deve ser compatível com Android e iOS. | Compatibilidade |
| RNF05 | O sistema deve garantir segurança dos dados do usuário (criptografia). | Segurança |
| RNF06 | O sistema deve ter suporte a acessibilidade (fonte grande, alto contraste, leitura por voz). | Acessibilidade |
| RNF07 | O sistema deve consumir pouca bateria do dispositivo. | Eficiência |
| RNF08 | O sistema deve armazenar dados localmente e/ou na nuvem com sincronização automática. | Armazenamento |
| RNF09 | O sistema deve suportar pelo menos 10.000 usuários simultâneos. | Escalabilidade |
| RNF10 | O sistema deve permitir backup automático dos dados. | Confiabilidade |
| RNF11 | O sistema deve seguir as diretrizes de privacidade de dados (ex: LGPD). | Conformidade |
| RNF12 | O sistema deve ter alta confiabilidade na execução dos alarmes (não pode falhar). | Confiabilidade |
| RNF13 | O sistema deve ter instalação simples e leve (tamanho reduzido do app). | Portabilidade |
| RNF14 | O sistema deve possuir linguagem clara e compreensível. | Usabilidade |

#####

## 📝 Casos de Uso

Os casos de uso representam as interações entre os diferentes tipos de usuários e o sistema, descrevendo suas funcionalidades principais.

O sistema foi projetado considerando dois tipos de atores principais:

⭢ Dependente (Conta Emparelhada)

⭢ Responsável

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

- Diagramas de Casos de Uso
  
[Clique aqui para ver os diagramas de casos de uso](https://github.com/mateusmtognoli/eng-software2-2026-1/tree/main/DOCS/CASOS%20DE%20USO)

####

## 🧩 Diagrama de Classes

O diagrama de classes apresenta a estrutura do sistema ReMed, descrevendo suas principais entidades, atributos e relacionamentos, modelados conforme os princípios da orientação a objetos e da UML tradicional.

---

- Principais Entidades:

O sistema é composto pelas seguintes classes principais:

⭢ Usuário

⭢ MetadadosUsuario

⭢ Dependente

⭢ Medicamento

⭢ ItemEstoque

⭢ EstatisticaAdesao

Além das enumerações:

⭢ StatusMedicamento

⭢ StatusEstoque

---

- Relacionamentos:


⭢ Um Usuário possui exatamente um conjunto de MetadadosUsuario, contendo informações complementares, como nome.

⭢ Um Usuário pode possuir zero ou vários Dependentes, sendo responsável pelo gerenciamento de seus dados.

⭢ Cada Dependente possui zero ou vários Medicamentos cadastrados para acompanhamento do tratamento.

⭢ Cada Dependente possui zero ou vários registros de EstatisticaAdesao, utilizados para acompanhar a adesão ao tratamento ao longo do tempo.

⭢ Cada Medicamento pode estar associado a zero ou um ItemEstoque, permitindo o controle da quantidade disponível do medicamento.

⭢ A classe Medicamento utiliza a enumeração StatusMedicamento para representar o estado atual da administração da dose (Pendente, Tomado, Atrasado ou Pulado).

⭢ A classe ItemEstoque utiliza a enumeração StatusEstoque para indicar a situação do estoque (Normal, Alerta ou Crítico).

---

- Observações Técnicas:

⭢ O modelo utiliza composição para representar relações de forte dependência entre as entidades, como entre Usuário e MetadadosUsuario, Dependente e Medicamento, e Dependente e EstatisticaAdesao.

⭢ O diagrama emprega associações com multiplicidades, evidenciando a cardinalidade dos relacionamentos entre as classes.

⭢ As enumerações StatusMedicamento e StatusEstoque foram modeladas como tipos específicos para garantir a consistência dos estados do sistema.

⭢ Os identificadores das entidades são representados por atributos do tipo String, podendo ser implementados utilizando UUID para assegurar unicidade.

⭢ O modelo contempla funcionalidades de gerenciamento de dependentes, controle de medicamentos, monitoramento da adesão ao tratamento e controle de estoque, servindo como base para a implementação do sistema ReMed.

---

[Clique aqui para acessar o diagrama de classes](DOCS/Diagrama-de-Classes-ReMed.png)

####

## 💻 Prototipação

A prototipação do sistema foi realizada com o objetivo de visualizar a interface do usuário e validar a experiência antes da implementação.

Foram desenvolvidos protótipos de alta fidelidade, representando as principais telas do sistema, como:

   ⭢ Tela de login e cadastro

   ⭢ Dashboard do usuário

   ⭢ Cadastro de medicamentos

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
