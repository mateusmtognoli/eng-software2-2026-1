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

O sistema foi projetado considerando quatro tipos de atores:

⭢ Paciente (Independente)

⭢ Paciente Dependente

⭢ Responsável

⭢ Administrador

---

- Paciente (Independente)

O paciente independente possui controle total sobre suas ações dentro do sistema:

⭢ UC01: Visualizar lista diária de medicamentos

⭢ UC02: Confirmar ingestão de medicamento

⭢ UC03: Visualizar histórico de ingestão

⭢ UC04: Configurar lembretes (som/vibração)

---

- Paciente Dependente

O paciente dependente possui interações mais limitadas e assistidas:

⭢ UCD01: Receber notificação de medicamento

⭢ UCD02: Confirmar ingestão via notificação

⭢ UCD03: Visualizar lista diária (somente leitura)

⭢ UCD04: Receber alerta recorrente (caso não confirme)

---

- Responsável

O responsável atua no acompanhamento e gestão dos pacientes dependentes:

⭢ UC01: Criar conta

⭢ UC02: Fazer login

⭢ UC03: Visualizar dashboard

⭢ UC04: Cadastrar medicamento

⭢ UC05: Visualizar histórico

⭢ UC06: Gerar relatório mensal

⭢ UC07: Visualizar dashboard do dependente

⭢ UC08: Gerenciar dependentes

⭢ UC09: Gerenciar rede de cuidado

---

🛠️ Administrador

O administrador é responsável pela gestão e manutenção do sistema:

⭢ UC12: Monitorar desempenho do sistema

⭢ UC13: Realizar manutenção e atualizações

⭢ UC14: Garantir segurança dos dados

⭢ UC15: Configurar backup automático

---

- Diagramas de Casos de Uso
  
[Clique aqui para ver os diagramas de casos de uso](DOCS/CASOS_DE_USO)

####

## 🧩 Diagrama de Classes

O diagrama de classes apresenta a estrutura do sistema, incluindo suas entidades, atributos, métodos e relacionamentos.

---

- Principais Entidades

O sistema é composto pelas seguintes classes principais:

⭢ Usuário (classe base)

⭢ Dependente

⭢ Responsável

⭢ Administrador

⭢ Medicamento

⭢ LembreteDose

⭢ RegistroDose

⭢ EstoqueMedicamento

⭢ Notificação

⭢ RelatorioAdesao

⭢ FichaMedica

⭢ Instituição

---

- Relacionamentos
  
⭢ A classe Usuário possui herança para Dependente, Responsável e Administrador

⭢ Um Dependente possui uma Ficha Médica

⭢ Um Medicamento está associado a lembretes e registros de dose

⭢ O sistema gera Notificações para os usuários

⭢ Dados de uso são consolidados em Relatórios de Adesão

⭢ O Administrador gerencia o sistema e suas configurações

---

- Observações Técnicas
  
⭢ O modelo utiliza conceitos de herança, composição e agregação

⭢ Os identificadores são baseados em UUID

⭢ O sistema contempla controle de estoque, notificações e relatórios

---

[Clique aqui para acessar o diagrama de classes](DOCS/diagrama_classes_remed.png)

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

![Dashboard do Usuário](https://github.com/mateusmtognoli/eng-software2-2026-1/blob/main/DOCS/IMAGENS%20PROTOTIPO/tela-inicial-remed.png)
![Dashboard do Administrador](https://github.com/mateusmtognoli/eng-software2-2026-1/blob/main/DOCS/IMAGENS%20PROTOTIPO/tela-inicial-remed-administrador.png)

---

- Acesso ao Protótipo

Caso queira visualizar o protótipo completo, acesse:

[Protótipo - Versão Usuários](https://ais-pre-4j3ii52jwzrkr4q653denk-157702196272.us-west2.run.app)

[Protótipo - Versão Administrador](https://stitch.withgoogle.com/preview/12183420891408613794?node-id=bdce2ebd1bd34224964dc9ea0783f5f6)

####

## 🛠️ Tecnologias Utilizadas (Futuramente)

- Frontend: React Native
- Backend: TypeScript
- Banco de Dados: MySQL / SQLite

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
