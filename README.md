# 💊 ReMed - Sistema de Gerenciamento de Medicamentos

  ![Engenharia de Software](https://img.shields.io/badge/Engenharia%20de%20Software-II-green)
  ![Status](https://img.shields.io/badge/status-em%20desenvolvimento-orange)

## 📌 Descrição

⭢ O ReMed é um aplicativo desenvolvido para auxiliar usuários — especialmente idosos e seus cuidadores — no controle do uso correto de medicamentos.

⭢ O sistema permite cadastrar remédios, configurar alarmes, enviar notificações e registrar o histórico de ingestão, garantindo mais segurança e organização no tratamento.

#####

## 🎯 Objetivos

⭢ Garantir o uso correto dos medicamentos  
⭢ Reduzir esquecimentos e falhas no tratamento  
⭢ Facilitar o acompanhamento por cuidadores  
⭢ Melhorar a organização da rotina de medicação  
⭢ Aumentar a segurança e autonomia do paciente  
⭢ Oferecer uma interface simples e acessível  

#####

## 👥 Atores / Personas

[Ver Personas](https://github.com/mateusmtognoli/eng-software2-2026-1/issues/1)

### 🧓 Paciente

⭢ Utiliza o sistema para controlar seus medicamentos  
⭢ Recebe alertas nos horários corretos  
⭢ Confirma a ingestão dos remédios  
⭢ Precisa de uma interface simples e acessível  
⭢ Pode visualizar seu histórico de uso  

---

### 👨‍⚕️ Cuidador / Responsável

⭢ Acompanha o uso de medicamentos do paciente  
⭢ Recebe notificações caso o medicamento não seja tomado  
⭢ Auxilia na organização da rotina de medicação  
⭢ Monitora o histórico de ingestão  
⭢ Pode gerenciar medicamentos do paciente  

---

### 👩‍💻 Administrador

⭢ Gerencia o funcionamento geral do sistema  
⭢ Monitora desempenho e disponibilidade  
⭢ Analisa dados e indicadores de uso  
⭢ Garante segurança e integridade dos dados  
⭢ Realiza manutenção e atualizações do sistema  

####

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
| RNF15 | O sistema deve suportar múltiplos idiomas (português, inglês, etc.). | Internacionalização |

#####

## 📝 Casos de Uso

[Ver Casos de Uso](adicionarlinkaqui)

####

## 👥 Público-Alvo

⭢ Idosos

⭢ Pacientes em tratamento contínuo

⭢ Cuidadores e familiares

#####

## 🛠️ Tecnologias Utilizadas (Futuramente)

- Frontend: React Native
- Backend: TypeScript
- Banco de Dados: MySQL

####

## 💻Protótipo

[Ver Protótipo](adicionarlinkdoprototipo)

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
